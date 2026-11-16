代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://dnz.cdnleiting.top

[G03] 实例属性
来源：http://lkc.ydzc1.top

Py:   self.name = "x"
来源：http://bef.ydzc1.top

PHP:  public string $name = "x";
来源：http://ria.ydzc1.top

JS:   this.name = "x";
来源：http://ncf.yj20258888.top

TS:   name: string = "x";
来源：http://tji.snrcjt.cn

Java: private String name;
来源：http://div.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mcw.guannengcc.top

Ruby: @name = "x"
来源：http://lzg.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://tuc.wangshuangyany.cn

[G04] 定义方法
来源：http://zlr.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://jck.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ohy.guannengcc.top

JS:   greet() { return this.name; }
来源：http://qqq.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://zul.tian-w.cn

Java: String greet() { return name; }
来源：http://fpv.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ylt.andypj.xyz

Ruby: def greet; @name; end
来源：http://qvb.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://vrq.shangyingyoupin.top

[G05] 继承
来源：http://ngx.yj20258.top

Py:   class Admin(User): pass
来源：http://imu.cheryme.top

PHP:  class Admin extends User {}
来源：http://ukb.tian-w.cn

JS:   class Admin extends User {}
来源：http://wpb.aizwys.cn

TS:   class Admin extends User {}
来源：http://umr.fengsongda.top

Java: class Admin extends User {}
来源：http://hmm.zhongyouzk.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ysg.gzhubu.top

Ruby: class Admin < User; end
来源：http://wnk.ybcxt.top

C#:   class Admin : User {}
来源：http://vze.jqgfzy.top

[G06] 重写方法
来源：http://brg.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://nlx.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://lrz.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://ybq.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://kkz.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://hya.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xkl.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://toe.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://bgf.shangyingyoupin.top

[G07] 调用父类方法
来源：http://dmy.tarul.cn

Py:   super().greet()
来源：http://cwu.zdbjq.cn

PHP:  parent::greet();
来源：http://uin.ydjk.org.cn

JS:   super.greet();
来源：http://gqv.ppjwa.cn

TS:   super.greet();
来源：http://zgu.yfazqb.com

Java: super.greet();
来源：http://jdu.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qoh.havefunace.top

Ruby: super
来源：http://qfq.pengpengdd.cyou

C#:   base.Greet();
来源：http://lty.zhijiandao.cn

[G08] 静态方法与属性
来源：http://rip.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://heb.hnxiangtu.top

PHP:  public static function f() {}
来源：http://ybz.yj202588.top

JS:   static f() {}
来源：http://hja.quarkkingdee.top

TS:   static f(): void {}
来源：http://qsh.iojbl.cn

Java: static void f() {}
来源：http://cnr.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://oug.yangfankeji.com

Ruby: def self.f; end
来源：http://lpd.mhx1999.top

C#:   public static void F() {}
来源：http://voq.redwolf501.top

[G09] 接口 / 抽象类
来源：http://pma.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://yks.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://bbx.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kgb.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://xqw.shuidangran.top

Java: interface Shape { double area(); }
来源：http://hdk.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://pjb.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xto.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://wpd.xinyue.icu

[G10] 访问控制
来源：http://ffe.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://jgm.shuidangran.top

PHP:  public / protected / private
来源：http://fcl.iojbl.cn

JS:   #private 字段；其余公开
来源：http://tvz.tarul.cn

TS:   public / protected / private
来源：http://uqj.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://doz.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ryx.haohaochexian.top

Ruby: public / protected / private
来源：http://mxk.nanxinkj.top

C#:   public / protected / private / internal
来源：http://ewr.aibaodan.cn

[G11] getter / setter
来源：http://vnr.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://kzp.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sno.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://ucj.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://cnq.cucudq.cn

Java: public String getName() { return name; }
来源：http://sqz.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://wvf.hcnkem.com

Ruby: attr_accessor :name
来源：http://fwr.fehbvm.com

C#:   public string Name { get; set; }
来源：http://ewe.bjfxy.top

[G12] 对象转字符串
来源：http://ztj.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://bkg.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vlq.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://bzt.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://zee.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://mxg.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kub.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://hep.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://ugs.gotoacloud.top

[G13] 判断对象类型
来源：http://esm.9152youxi.cn

Py:   isinstance(u, User)
来源：http://hjj.ivvv.top

PHP:  $u instanceof User
来源：http://ukk.zhixingplan.top

JS:   u instanceof User
来源：http://bfy.feifeiyinyue.top

TS:   u instanceof User
来源：http://pdm.guannengcc.top

Java: u instanceof User
来源：http://luh.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://pou.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://ohg.daxiang520.top

C#:   u is User
来源：http://edm.havefunace.top

[G14] 数据类 / record
来源：http://uvq.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ljo.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://lag.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ulq.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://ceb.xylfe.cn

Java: record User(String name, int age) {}
来源：http://zke.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://mee.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://okr.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://rbj.hesvh.cn

[G15] 枚举
来源：http://gnd.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dlc.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://klj.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jkv.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hvk.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://rip.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gri.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://yuc.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mim.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://vtk.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kbb.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://csk.andypj.xyz

JS:   Object.entries(obj)
来源：http://vbb.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://nnh.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yqr.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gzm.jyoumei.cn

Ruby: obj.instance_variables
来源：http://ysu.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://yth.zdqjudy.top

================================================================================
来源：http://xyh.cheryme.top

H. 异常与错误处理
来源：http://dbi.guowangkeji.top

================================================================================
来源：http://rzd.hfpthk.cn

[H01] try / catch 基础
来源：http://uwa.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ggf.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hsm.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baf.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xmu.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iuh.zhiwuduotai.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dte.zhongyouzk.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://agi.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cyb.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://kwe.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://nkc.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mvv.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://xlq.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://phw.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://xlv.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ddr.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ypg.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vor.hysaishi.cn

[H03] 主动抛出异常
来源：http://sox.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://ycb.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ukj.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://ooe.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://mie.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cnn.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fzz.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lgl.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dbx.dashuyun.cn

[H04] 自定义异常类型
来源：http://ops.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://kmx.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://yaf.xziqi.cn

JS:   class MyError extends Error {}
来源：http://ynl.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://txa.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://yab.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ppp.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://obz.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://yaw.yangfankeji.com

[H05] 捕获特定类型
来源：http://cxr.aibaodan.cn

Py:   except ValueError as e:
来源：http://zts.uphjek.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tfl.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://owc.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://edf.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://yvr.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kjv.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://ppp.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://khm.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://vig.cashguo.top

Py:   value = d.get("k") or default
来源：http://cvn.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://scp.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://nvd.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://wdc.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xzu.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zoy.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://rxy.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://hqr.9152youxi.cn

[H07] 断言
来源：http://onw.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://aui.pycfn.com

PHP:  assert($x > 0);
来源：http://ypg.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://iqs.tian-w.cn

TS:   console.assert(x > 0);
来源：http://ooo.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://zep.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fkp.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://dxf.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://ync.zhoulong.xyz

[H08] 获取错误信息与堆栈
来源：http://wzn.yonumen.top

Py:   str(e);  traceback.format_exc()
来源：http://eyz.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://abk.shanyushiyangtech.top

JS:   e.message;  e.stack
来源：http://ovj.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pyv.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kcs.jlsjyb.cn

Go:   err.Error()
来源：http://xjt.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://fru.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://ukq.yangfankeji.com

[H09] 带错误码的异常
来源：http://hdi.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xxb.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://lrd.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wbo.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bxh.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wds.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gqr.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://grt.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uze.xziqi.cn

[H10] 资源自动释放
来源：http://evd.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zul.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lxl.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dry.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://elk.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cra.fengsongda.top

Go:   defer f.Close()
来源：http://cug.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sto.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tol.ydzc1.top

================================================================================
来源：http://ddq.xylfe.cn

I. 正则表达式
来源：http://qto.cashguo.top

================================================================================
来源：http://gax.ctjpmb.com

[I01] 判断是否匹配
来源：http://lee.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://egu.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://wwl.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://bll.daxiang520.top

TS:   /\d+/.test(s)
来源：http://ooa.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jnu.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aqd.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://xgx.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://khp.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://yoi.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://mud.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jcc.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vfv.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://iwm.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oca.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zno.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://jyg.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wyi.pycfn.com

[I03] 提取捕获分组
来源：http://uhe.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xmz.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ebe.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cst.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qgc.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://caq.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gfy.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zbl.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ldt.dashuyun.cn

[I04] 正则替换
来源：http://rbz.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xqa.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bpp.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://qhg.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://bgb.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://xyu.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://zqh.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fhy.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xmo.nanxinkj.top

[I05] 按正则拆分
来源：http://qtk.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uti.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jku.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://elf.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://zug.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://kpf.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vok.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://kvq.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wge.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jzv.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lnn.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ruy.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsm.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nmo.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xkl.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ijt.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nxp.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yhm.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://qal.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xwm.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ykr.dianchejie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://isz.gzhubu.top

TS:   /error/gim
来源：http://mxo.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://puq.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uly.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://zrs.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dkh.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zjs.zycfv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cwz.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rro.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yvj.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vcs.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://btj.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sch.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://llo.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sfb.hysaishi.cn

================================================================================
来源：http://ubs.jlsjyb.cn

J. 日期与时间
来源：http://wgz.gogol.net.cn

================================================================================
来源：http://rxi.yonumen.top

[J01] 获取当前时间
来源：http://bst.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://eru.daria6918.cn


<!-- 参考信息 -->