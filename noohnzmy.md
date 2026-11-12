代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://don.hnqzz.top

[G03] 实例属性
来源：http://nve.hnqzz.top

Py:   self.name = "x"
来源：http://lzd.sxryk.cn

PHP:  public string $name = "x";
来源：http://tpn.hesvh.cn

JS:   this.name = "x";
来源：http://xul.52xcode.cn

TS:   name: string = "x";
来源：http://qje.yueranfly.top

Java: private String name;
来源：http://qnj.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bqa.tianlin.xyz

Ruby: @name = "x"
来源：http://wuq.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://znd.snrcjt.cn

[G04] 定义方法
来源：http://sjn.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://nrd.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ijp.yonumen.top

JS:   greet() { return this.name; }
来源：http://hhh.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://hij.hywenlv.cn

Java: String greet() { return name; }
来源：http://gwp.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mwn.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://hbv.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://oru.zhixingplan.top

[G05] 继承
来源：http://jvf.pycfn.com

Py:   class Admin(User): pass
来源：http://qea.andypj.xyz

PHP:  class Admin extends User {}
来源：http://elm.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://dkl.havefunace.top

TS:   class Admin extends User {}
来源：http://gqs.daxiang520.top

Java: class Admin extends User {}
来源：http://poc.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bam.fktsv.cn

Ruby: class Admin < User; end
来源：http://hgn.andypj.xyz

C#:   class Admin : User {}
来源：http://cfi.316326.xyz

[G06] 重写方法
来源：http://xuf.birdmap.top

Py:   def greet(self): return "admin"
来源：http://jpl.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://icn.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://jfp.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://ctp.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://ooj.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cpl.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://vkw.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://kro.cheryme.top

[G07] 调用父类方法
来源：http://lrj.jqgufenzy.top

Py:   super().greet()
来源：http://vfs.jlsjyb.cn

PHP:  parent::greet();
来源：http://knc.cashguo.top

JS:   super.greet();
来源：http://kor.jinghuilouyu.cn

TS:   super.greet();
来源：http://kdv.jinqigufen.top

Java: super.greet();
来源：http://znt.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zzo.yanxiufei.cn

Ruby: super
来源：http://gop.xuetiantiany.cn

C#:   base.Greet();
来源：http://uad.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://ehd.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://erw.yangfankeji.com

PHP:  public static function f() {}
来源：http://use.gotoacloud.top

JS:   static f() {}
来源：http://jpr.zhongyouzk.top

TS:   static f(): void {}
来源：http://xcd.shanyushiyangkeji.top

Java: static void f() {}
来源：http://mlu.aibaodan.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://spz.epnwcf.com

Ruby: def self.f; end
来源：http://nba.smart0.xyz

C#:   public static void F() {}
来源：http://lgi.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://orr.jqgfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://tlg.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://slw.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://foh.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://jnz.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://ghv.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://lxz.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://icj.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://okr.epnwcf.com

[G10] 访问控制
来源：http://sep.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://jnx.epnwcf.com

PHP:  public / protected / private
来源：http://xzp.sxryk.cn

JS:   #private 字段；其余公开
来源：http://jrj.quarkkingdee.top

TS:   public / protected / private
来源：http://dnh.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://ihe.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dfi.jinqigufen.top

Ruby: public / protected / private
来源：http://ruo.tarul.cn

C#:   public / protected / private / internal
来源：http://plh.jlsjyb.cn

[G11] getter / setter
来源：http://bfq.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://yga.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yrr.wangdashe.top

JS:   get name() { return this._name; }
来源：http://qso.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://oua.cqqwz.cn

Java: public String getName() { return name; }
来源：http://kzw.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dxf.sxryk.cn

Ruby: attr_accessor :name
来源：http://crg.mhx1999.top

C#:   public string Name { get; set; }
来源：http://iim.hfpthk.cn

[G12] 对象转字符串
来源：http://obx.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://jco.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://sog.andypj.xyz

JS:   toString() { return this.name; }
来源：http://iwh.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://pva.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://vmr.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kob.gaohongyu789.top

Ruby: def to_s; @name; end
来源：http://wju.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://edd.yanxiufei.cn

[G13] 判断对象类型
来源：http://ytr.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://pjw.aizwys.cn

PHP:  $u instanceof User
来源：http://uuy.ctjpmb.com

JS:   u instanceof User
来源：http://pkn.fktsv.cn

TS:   u instanceof User
来源：http://vks.gotoacloud.top

Java: u instanceof User
来源：http://ori.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://vof.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://hmc.yangfankeji.com

C#:   u is User
来源：http://fef.guowangkeji.top

[G14] 数据类 / record
来源：http://nbq.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sqb.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://yiq.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://sok.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://yvd.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://qgo.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://akt.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xbn.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://wfd.xingfuxueyuan.xyz

[G15] 枚举
来源：http://nqh.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uqh.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ebj.yj20258.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eri.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://obs.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://vez.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dqy.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://osi.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sie.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://nts.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qfp.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://mem.yonumen.top

JS:   Object.entries(obj)
来源：http://lcz.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://lzq.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mpe.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ino.vehdjk.com

Ruby: obj.instance_variables
来源：http://fha.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://qzm.fanxiaobao.xyz

================================================================================
来源：http://srv.c1oappe.top

H. 异常与错误处理
来源：http://fea.ybcxt.top

================================================================================
来源：http://mta.fzhhl.top

[H01] try / catch 基础
来源：http://nvc.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vbp.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vux.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oos.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kze.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://obz.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mej.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qhn.mhx1999.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bth.yonumen.top

[H02] finally / ensure 收尾
来源：http://qxg.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://ydb.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://mjc.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gtx.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hav.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lxp.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pvy.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lxj.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://irr.yj20258888.top

[H03] 主动抛出异常
来源：http://cbm.shanyushiyangtech.top

Py:   raise ValueError("错误信息")
来源：http://lfx.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xno.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://izw.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://byb.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ijt.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wua.hcnkem.com

Ruby: raise ArgumentError, "错误信息"
来源：http://gep.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qiz.sxryk.cn

[H04] 自定义异常类型
来源：http://hva.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://xyo.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ulj.yj20258.top

JS:   class MyError extends Error {}
来源：http://nmz.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://udg.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://dus.cqqwz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfx.xingfuxueyuan.xyz

Ruby: class MyError < StandardError; end
来源：http://eko.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://eqp.fzhhl.top

[H05] 捕获特定类型
来源：http://rej.yuanzhike.top

Py:   except ValueError as e:
来源：http://epf.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tiq.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://gfs.jlsjyb.cn

TS:   if (e instanceof TypeError) {}
来源：http://ahk.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://mbh.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ulw.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://bqu.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ppg.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://hxd.aizwys.cn

Py:   value = d.get("k") or default
来源：http://qzy.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://fpm.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://kvh.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://hfq.shuidangran.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cbw.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fja.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://gqz.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://tnc.shangyingyoupin.top

[H07] 断言
来源：http://imk.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://vyo.yongpay.top

PHP:  assert($x > 0);
来源：http://wei.tarul.cn

JS:   console.assert(x > 0);
来源：http://aev.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://nin.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://yxp.redwolf501.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mgd.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://dcy.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://gyy.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://mgp.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://fdr.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vcx.yvedp.cn

JS:   e.message;  e.stack
来源：http://dho.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://owv.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gdm.chenjidiqi.icu

Go:   err.Error()
来源：http://cly.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://jfd.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://xap.9152youxi.cn

[H09] 带错误码的异常
来源：http://fas.mhx1999.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nev.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tel.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://umh.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dyv.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jzo.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bxe.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://mnm.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://beh.shuidangran.top

[H10] 资源自动释放
来源：http://uum.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lov.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ecv.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nkm.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lsd.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cmt.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://yii.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bbl.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://szt.sufxvd.cn

================================================================================
来源：http://jgm.aibaodan.cn

I. 正则表达式
来源：http://jut.jqgufenzy.top

================================================================================
来源：http://olq.aizwys.cn

[I01] 判断是否匹配
来源：http://ukp.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://awa.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rqi.hcnkem.com

JS:   /\d+/.test(s)
来源：http://tcw.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://wac.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://smc.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pax.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://ats.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://khl.fzhhl.top

[I02] 提取所有匹配
来源：http://buo.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://srh.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pxq.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lit.yonumen.top

TS:   s.match(/\d+/g)
来源：http://pbp.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://opd.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://men.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://qzx.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nfs.yanxiufei.cn

[I03] 提取捕获分组
来源：http://udp.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zct.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jcq.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qnr.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oce.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ikh.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gjz.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cof.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eef.yongpay.top

[I04] 正则替换
来源：http://kvq.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gwm.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tuo.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://grs.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://qoy.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://cvx.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oad.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aki.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mon.gotoacloud.top

[I05] 按正则拆分
来源：http://bsc.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://akb.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://emu.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://lky.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://ybh.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://ypv.aibaodan.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yyx.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fcn.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wfl.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jrp.nwbrower.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ebo.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://alm.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhi.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pae.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oyu.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mpx.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lsp.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aph.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://mvd.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sbs.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wlk.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wjo.hfpthk.cn

TS:   /error/gim
来源：http://aeq.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hpo.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nau.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://few.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://npc.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://bdj.yj20258.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nza.gzhubu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ngj.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kxe.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ktt.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://szc.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mxc.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ozx.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jgv.pengpengdd.cyou

================================================================================
来源：http://dbo.gogol.net.cn

J. 日期与时间
来源：http://iif.chenjidiqi.icu

================================================================================
来源：http://lxh.aibaodan.cn

[J01] 获取当前时间
来源：http://wyf.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://oer.yuanzhike.top


<!-- 参考信息 -->