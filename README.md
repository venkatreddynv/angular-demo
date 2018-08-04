# angular-demo

import { Component, OnInit } from '@angular/core';
import { Router, ActivatedRoute } from '@angular/router';
import { User } from '../model/login.model';
import { AuthenticationService } from '../services/authentication.service';

@Component({

  selector: 'app-login-form',
  templateUrl: './login-form.component.html',
  styleUrls: ['./login-form.component.css']
})
export class LoginFormComponent implements OnInit {

  model: User = new User();
  alert = '';
  isValid = false;
  onClickMe() {
