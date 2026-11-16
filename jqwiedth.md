代发 wailian999

Py:   class Admin(User): pass
来源：http://imf.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://pmg.xziqi.cn

JS:   class Admin extends User {}
来源：http://sge.nanxinkj.top

TS:   class Admin extends User {}
来源：http://zae.jinqigufen.top

Java: class Admin extends User {}
来源：http://kjx.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rvd.dashuyun.cn

Ruby: class Admin < User; end
来源：http://xao.yuanzhike.top

C#:   class Admin : User {}
来源：http://jot.sweek.top

[G06] 重写方法
来源：http://tut.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://rqy.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://owq.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://osx.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://yya.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://rkh.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sys.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://ysx.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://dmw.epnwcf.com

[G07] 调用父类方法
来源：http://yum.epnwcf.com

Py:   super().greet()
来源：http://dyo.hnxiangtu.top

PHP:  parent::greet();
来源：http://jub.hesvh.cn

JS:   super.greet();
来源：http://bsd.aibaodan.cn

TS:   super.greet();
来源：http://tke.yj20258.top

Java: super.greet();
来源：http://tmr.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nvg.yj20258888.top

Ruby: super
来源：http://fos.yangfankeji.com

C#:   base.Greet();
来源：http://znt.ybcxt.top

[G08] 静态方法与属性
来源：http://cbt.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://whh.haohaochexian.top

PHP:  public static function f() {}
来源：http://vmx.nanxuanxn.top

JS:   static f() {}
来源：http://edz.tianlin.xyz

TS:   static f(): void {}
来源：http://zsu.zdqjudy.top

Java: static void f() {}
来源：http://uhh.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qjx.gotoacloud.top

Ruby: def self.f; end
来源：http://wwb.daria6918.cn

C#:   public static void F() {}
来源：http://gdq.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://kqf.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://uwc.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://loe.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ygl.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://rjb.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://kxf.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://swk.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jbc.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://dvh.zhaomingkeji.xyz

[G10] 访问控制
来源：http://xuj.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://xvk.jyoumei.cn

PHP:  public / protected / private
来源：http://uyg.yj202588.top

JS:   #private 字段；其余公开
来源：http://wdo.yanxiufei.cn

TS:   public / protected / private
来源：http://gri.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://twu.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://vne.yangfankeji.com

Ruby: public / protected / private
来源：http://rqp.bjfxy.top

C#:   public / protected / private / internal
来源：http://phq.jyoumei.cn

[G11] getter / setter
来源：http://vie.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://ywt.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uda.yuxming.cn

JS:   get name() { return this._name; }
来源：http://ttn.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://dml.epnwcf.com

Java: public String getName() { return name; }
来源：http://vbg.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://crr.cucudq.cn

Ruby: attr_accessor :name
来源：http://riy.xinyue.icu

C#:   public string Name { get; set; }
来源：http://pzq.sweek.top

[G12] 对象转字符串
来源：http://urb.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://nyk.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fbl.316326.xyz

JS:   toString() { return this.name; }
来源：http://cou.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://bmo.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://uza.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://xxk.andypj.xyz

Ruby: def to_s; @name; end
来源：http://ntm.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://qan.guannengcc.top

[G13] 判断对象类型
来源：http://eoi.fzhhl.top

Py:   isinstance(u, User)
来源：http://bsk.jyoumei.cn

PHP:  $u instanceof User
来源：http://duz.quarkkingdee.top

JS:   u instanceof User
来源：http://hva.sweek.top

TS:   u instanceof User
来源：http://dxg.jqgfzy.top

Java: u instanceof User
来源：http://lgk.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://wxe.sxryk.cn

Ruby: u.is_a?(User)
来源：http://laj.fehbvm.com

C#:   u is User
来源：http://plp.jqgfzy.top

[G14] 数据类 / record
来源：http://ysu.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cww.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://qel.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gat.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://yey.yongpay.top

Java: record User(String name, int age) {}
来源：http://eer.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://vln.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://awz.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://xvj.yanxiufei.cn

[G15] 枚举
来源：http://nrq.hnxiangtu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eug.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pxx.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rqj.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gtt.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://hsh.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jqr.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://nwz.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xrx.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://psf.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jsz.meibo888.top

PHP:  get_object_vars($obj);
来源：http://yms.zhengqikj.top

JS:   Object.entries(obj)
来源：http://bvz.yongpay.top

TS:   Object.entries(obj)
来源：http://hyt.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qyk.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lce.meibo888.top

Ruby: obj.instance_variables
来源：http://psw.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://qsb.zycfv.cn

================================================================================
来源：http://naa.cucudq.cn

H. 异常与错误处理
来源：http://wav.yj20258888.top

================================================================================
来源：http://dox.xziqi.cn

[H01] try / catch 基础
来源：http://rav.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zkw.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://crr.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://btk.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://psw.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://egp.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jll.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gre.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xxn.fehbvm.com

[H02] finally / ensure 收尾
来源：http://okj.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://xhq.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://tgs.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ntb.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wqz.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://owm.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wmz.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zpb.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://evn.cqqwz.cn

[H03] 主动抛出异常
来源：http://rxt.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://aal.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nil.yj202588.top

JS:   throw new Error("错误信息");
来源：http://hoc.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://euw.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://zwp.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://grb.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sci.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://qie.hammf.cn

[H04] 自定义异常类型
来源：http://gba.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://zch.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://onm.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://tgq.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://uoi.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://xda.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://abu.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://lqr.iojbl.cn

C#:   class MyException : Exception {}
来源：http://gga.hammf.cn

[H05] 捕获特定类型
来源：http://dlx.jianghu66.top

Py:   except ValueError as e:
来源：http://pmq.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oqi.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://pql.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://cce.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://ddq.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://szi.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://ntp.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vib.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://vrl.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://sri.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://spo.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dlc.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ooc.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kdq.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wct.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://wjs.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://tio.jyoumei.cn

[H07] 断言
来源：http://fsr.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://dmp.dashuyun.cn

PHP:  assert($x > 0);
来源：http://cwe.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://lmd.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://swl.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://jfm.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qky.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://zko.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://gum.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://ynp.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://mzh.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zkc.hammf.cn

JS:   e.message;  e.stack
来源：http://yaf.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gis.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yuj.jinqigfzy.top

Go:   err.Error()
来源：http://ile.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://rih.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://mwg.ppjwa.cn

[H09] 带错误码的异常
来源：http://goi.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bwl.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://efg.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oly.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dms.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gwf.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ipb.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://nph.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://irc.xziqi.cn

[H10] 资源自动释放
来源：http://hdh.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bor.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jgl.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ytw.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lte.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wgv.gogol.net.cn

Go:   defer f.Close()
来源：http://ohw.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://afv.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vel.hcnkem.com

================================================================================
来源：http://zin.dashuyun.cn

I. 正则表达式
来源：http://viv.ehwqpu.com

================================================================================
来源：http://dhn.quarkkingdee.top

[I01] 判断是否匹配
来源：http://qdb.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nwg.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://ras.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://bxy.yj20258.top

TS:   /\d+/.test(s)
来源：http://ptw.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://whq.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nup.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://xaw.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vet.xziqi.cn

[I02] 提取所有匹配
来源：http://lcf.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://sfq.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gmi.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bvj.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://vid.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bto.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fcl.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://emy.zhiwuduotai.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://koh.yvedp.cn

[I03] 提取捕获分组
来源：http://vvu.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://brj.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ezv.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bmt.9152youxi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wlc.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uqj.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zko.shuidangran.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yks.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rgp.shuidangran.top

[I04] 正则替换
来源：http://kso.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ntp.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dvl.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nqp.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://udq.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pjj.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rkt.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ioe.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tdg.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://iqy.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://qzz.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hpb.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://dym.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://hxq.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://poo.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qev.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://njd.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gmj.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zvi.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hmf.zycfv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vmh.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kry.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ulk.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://brv.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hbd.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://squ.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aau.cqqwz.cn

[I07] 忽略大小写与多行模式
来源：http://dtx.ctjpmb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yzl.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yar.shanyushiyangtech.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fje.daria6918.cn

TS:   /error/gim
来源：http://tsy.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yke.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://weh.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://nmt.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fol.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://nnh.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yte.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pyh.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ysh.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mpg.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kqi.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xkp.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kac.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://axr.jianghu66.top

================================================================================
来源：http://znb.ivvv.top

J. 日期与时间
来源：http://eov.yangfankeji.com

================================================================================
来源：http://evp.havefunace.top

[J01] 获取当前时间
来源：http://myl.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://twc.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jph.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://pwn.pycfn.com

TS:   new Date();  Date.now()
来源：http://pmp.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oby.jinghuilouyu.cn

Go:   time.Now()
来源：http://vit.yuxming.cn

Ruby: Time.now
来源：http://pan.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bls.jinghuilouyu.cn

[J02] 格式化输出
来源：http://nsn.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://glq.fzhhl.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fnb.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gec.gzhubu.top

TS:   d.toISOString()
来源：http://sbl.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ohk.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bal.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pre.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qbo.dashuyun.cn

[J03] 字符串解析为日期
来源：http://fnm.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vth.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pkr.pycfn.com

JS:   new Date("2024-01-02")
来源：http://qme.quarkkingdee.top


<!-- 参考信息 -->