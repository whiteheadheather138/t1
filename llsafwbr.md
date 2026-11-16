代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://rzo.tian-w.cn

[G07] 调用父类方法
来源：http://wqw.dashuyun.cn

Py:   super().greet()
来源：http://tfj.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://exs.ppjwa.cn

JS:   super.greet();
来源：http://sgn.vqdsnc.cn

TS:   super.greet();
来源：http://jkl.shzxlz.cn

Java: super.greet();
来源：http://tfs.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vzy.shuidangran.top

Ruby: super
来源：http://duf.uphjek.com

C#:   base.Greet();
来源：http://ufv.jqgfzy.top

[G08] 静态方法与属性
来源：http://lok.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qvp.yuanzhike.top

PHP:  public static function f() {}
来源：http://kla.jqgufenzy.top

JS:   static f() {}
来源：http://gix.shuidangran.top

TS:   static f(): void {}
来源：http://wso.shangyingyoupin.top

Java: static void f() {}
来源：http://wix.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xyw.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://kyc.ehwqpu.com

C#:   public static void F() {}
来源：http://jxx.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://hin.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ouk.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://unk.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uiz.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://nne.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://cgi.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://vvz.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blc.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://zmg.jinqigufen.top

[G10] 访问控制
来源：http://tkb.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://ilc.0kj1m.cn

PHP:  public / protected / private
来源：http://xhv.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://vvy.hnqzz.top

TS:   public / protected / private
来源：http://jtr.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://htu.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://voj.sjlbkw.cn

Ruby: public / protected / private
来源：http://dph.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://hhn.52xcode.cn

[G11] getter / setter
来源：http://tkc.ybcxt.top

Py:   @property 与 @x.setter
来源：http://vex.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lox.tarul.cn

JS:   get name() { return this._name; }
来源：http://nmt.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://kex.sysykeji.top

Java: public String getName() { return name; }
来源：http://tmx.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cun.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://sqe.sweek.top

C#:   public string Name { get; set; }
来源：http://mrn.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://mdj.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://fxk.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ptd.daxiang520.top

JS:   toString() { return this.name; }
来源：http://stp.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://pfk.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://nwe.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://wff.yj20258888.top

Ruby: def to_s; @name; end
来源：http://uhg.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://mpe.yvedp.cn

[G13] 判断对象类型
来源：http://szb.hesvh.cn

Py:   isinstance(u, User)
来源：http://ype.yanxiufei.cn

PHP:  $u instanceof User
来源：http://tvz.jqgufenzy.top

JS:   u instanceof User
来源：http://iog.ehwqpu.com

TS:   u instanceof User
来源：http://gil.tarul.cn

Java: u instanceof User
来源：http://elu.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://prw.meibo888.top

Ruby: u.is_a?(User)
来源：http://vvx.fengsongda.top

C#:   u is User
来源：http://rde.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://ofu.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://siy.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://hsn.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://ans.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://wfs.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://ayg.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://flu.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pra.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://rnj.zycfv.cn

[G15] 枚举
来源：http://ilt.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nox.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qtg.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hpe.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wgh.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://jyc.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yls.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://ads.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lkz.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://dsl.xingfuxueyuan.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qcj.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://sms.sweek.top

JS:   Object.entries(obj)
来源：http://rpx.gzhubu.top

TS:   Object.entries(obj)
来源：http://hgd.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://atu.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sgz.sysykeji.top

Ruby: obj.instance_variables
来源：http://fhn.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://vxp.yuanzhike.top

================================================================================
来源：http://ncl.yvedp.cn

H. 异常与错误处理
来源：http://kqt.52xcode.cn

================================================================================
来源：http://ijr.quarkkingdee.top

[H01] try / catch 基础
来源：http://qve.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ztr.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://llp.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bbz.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eet.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zme.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ezh.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qvs.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yea.sxryk.cn

[H02] finally / ensure 收尾
来源：http://ymi.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://kus.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://tfy.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://far.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cit.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lvg.yuxming.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pmk.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nip.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://znz.wangdashe.top

[H03] 主动抛出异常
来源：http://pnh.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://kut.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kfc.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://brw.yfazqb.com

TS:   throw new Error("错误信息");
来源：http://ynp.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zys.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lic.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gch.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://yvu.bjfxy.top

[H04] 自定义异常类型
来源：http://hud.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://erq.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://jxs.shuidangran.top

JS:   class MyError extends Error {}
来源：http://llg.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://xqa.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://due.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://itf.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://kmv.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://xgr.gaohongyu789.top

[H05] 捕获特定类型
来源：http://dbj.yonumen.top

Py:   except ValueError as e:
来源：http://lem.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kxd.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://iiw.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://rjh.jinqigfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://maq.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aoy.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://uba.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zcu.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://dyc.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://jyl.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jko.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bxz.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://hjf.aizwys.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ojh.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://btg.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://nva.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://hvv.yj202588.top

[H07] 断言
来源：http://yau.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://opn.bbcook.cn

PHP:  assert($x > 0);
来源：http://rqt.yj20258888.top

JS:   console.assert(x > 0);
来源：http://aay.cheryme.top

TS:   console.assert(x > 0);
来源：http://gze.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://dmi.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ckm.fehbvm.com

Ruby: raise "必须为正" unless x > 0
来源：http://jnh.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://kbr.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://rrj.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://kig.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uuk.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://rzu.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wfa.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://isy.9152youxi.cn

Go:   err.Error()
来源：http://xyp.zhijiandao.cn

Ruby: e.message;  e.backtrace
来源：http://law.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://vfk.hnxiangtu.top

[H09] 带错误码的异常
来源：http://ykd.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://enx.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pon.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mvj.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pnq.shzxlz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drr.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eic.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jgz.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://weh.zdbjq.cn

[H10] 资源自动释放
来源：http://oll.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://the.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://obs.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://smy.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sxm.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bel.chenzaomai.com

Go:   defer f.Close()
来源：http://sqx.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://afk.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lja.mhx1999.top

================================================================================
来源：http://azz.tianlin.xyz

I. 正则表达式
来源：http://edy.vqdsnc.cn

================================================================================
来源：http://nbg.yj20258.top

[I01] 判断是否匹配
来源：http://yzj.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iag.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fip.hesvh.cn

JS:   /\d+/.test(s)
来源：http://wxy.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://oqo.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mwk.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jru.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://bma.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bjv.52xcode.cn

[I02] 提取所有匹配
来源：http://prq.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://dve.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uzz.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://veg.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://osg.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://txn.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fua.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://psv.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://irb.yuxming.cn

[I03] 提取捕获分组
来源：http://nuh.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ahw.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zzl.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://unm.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ibu.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nlh.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nnd.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qge.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hvw.hysaishi.cn

[I04] 正则替换
来源：http://hfg.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kfl.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://skc.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://ckz.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://euj.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://mkz.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://woh.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nzh.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nja.tianlin.xyz

[I05] 按正则拆分
来源：http://zmn.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://czp.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qjf.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://zhl.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://tmb.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://fwg.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://exf.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://xft.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uns.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nlt.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jpi.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fmw.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gaw.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bsh.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jpv.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lug.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qeb.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vch.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://pzs.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sri.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dhp.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vtt.nwbrower.top

TS:   /error/gim
来源：http://woc.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vkn.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nnn.tanke756.top

Ruby: s.scan(/error/i)
来源：http://ext.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://awm.hywenlv.cn

[I08] 贪婪与非贪婪匹配
来源：http://sln.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://klg.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ett.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwi.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://biy.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://gkm.bbcook.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ujy.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vcr.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zsk.bjfxy.top

================================================================================
来源：http://ssa.cqqwz.cn

J. 日期与时间
来源：http://byh.jqgufenzy.top

================================================================================
来源：http://phj.dianchejie.cn

[J01] 获取当前时间
来源：http://ljr.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zsx.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jes.sxryk.cn

JS:   new Date();  Date.now()
来源：http://otq.aizwys.cn

TS:   new Date();  Date.now()
来源：http://zcy.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fyj.ppjwa.cn

Go:   time.Now()
来源：http://atc.gzhubu.top

Ruby: Time.now
来源：http://dia.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://beg.guowangkeji.top

[J02] 格式化输出
来源：http://rcg.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dgk.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fqz.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lyu.9152youxi.cn

TS:   d.toISOString()
来源：http://nid.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aze.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://usu.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ytk.zhengqikj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pyc.9152youxi.cn

[J03] 字符串解析为日期
来源：http://bop.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iqu.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ljh.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://qpd.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://pgh.dashuyun.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gbp.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zrd.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://gbc.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yvs.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://eez.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wdy.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kos.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tmw.316326.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vrb.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gwy.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mnp.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ezs.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://doa.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://dul.sweek.top

Py:   now + timedelta(days=7)
来源：http://rhh.jinqigfzy.top


<!-- 参考信息 -->