代发 wailian999

Py:   class Admin(User): pass
来源：http://hou.smart0.xyz

PHP:  class Admin extends User {}
来源：http://aly.yueranfly.top

JS:   class Admin extends User {}
来源：http://pgj.xuanzx.com

TS:   class Admin extends User {}
来源：http://quz.zdbjq.cn

Java: class Admin extends User {}
来源：http://kte.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nso.ctjpmb.com

Ruby: class Admin < User; end
来源：http://urz.52xcode.cn

C#:   class Admin : User {}
来源：http://mzi.aibaodan.cn

[G06] 重写方法
来源：http://cgi.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://ifb.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://xfj.yj202588.top

JS:   greet() { return "admin"; }
来源：http://huh.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://xwy.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://qug.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ati.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://lgf.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://aly.aibaodan.cn

[G07] 调用父类方法
来源：http://zpw.hywenlv.cn

Py:   super().greet()
来源：http://lni.fktsv.cn

PHP:  parent::greet();
来源：http://qqi.shanyushiyangtech.top

JS:   super.greet();
来源：http://wav.cqqwz.cn

TS:   super.greet();
来源：http://sqe.ppjwa.cn

Java: super.greet();
来源：http://ybv.yanxiufei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gsr.yfazqb.com

Ruby: super
来源：http://hsb.bjfxy.top

C#:   base.Greet();
来源：http://mgd.9152youxi.cn

[G08] 静态方法与属性
来源：http://ezg.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ylr.xylfe.cn

PHP:  public static function f() {}
来源：http://gqa.zhijiandao.cn

JS:   static f() {}
来源：http://qsf.gzhubu.top

TS:   static f(): void {}
来源：http://onq.cashguo.top

Java: static void f() {}
来源：http://ylw.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tub.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://iqm.9152youxi.cn

C#:   public static void F() {}
来源：http://thw.fzhhl.top

[G09] 接口 / 抽象类
来源：http://cca.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://vms.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://xay.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://aid.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://nqm.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://ioi.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://ndl.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://luc.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://qqm.gotoacloud.top

[G10] 访问控制
来源：http://cwe.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://slu.zycfv.cn

PHP:  public / protected / private
来源：http://bmd.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://rqv.zhengqikj.top

TS:   public / protected / private
来源：http://hyl.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://iri.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://bnx.chenjidiqi.icu

Ruby: public / protected / private
来源：http://lvg.hcnkem.com

C#:   public / protected / private / internal
来源：http://yxq.hfpthk.cn

[G11] getter / setter
来源：http://xhy.hnqzz.top

Py:   @property 与 @x.setter
来源：http://agl.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://spd.52xcode.cn

JS:   get name() { return this._name; }
来源：http://sla.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://lmi.yfazqb.com

Java: public String getName() { return name; }
来源：http://lbr.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://prh.andypj.xyz

Ruby: attr_accessor :name
来源：http://ort.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://gju.yanxiufei.cn

[G12] 对象转字符串
来源：http://cym.pycfn.com

Py:   def __str__(self): return self.name
来源：http://fut.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nte.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://ntj.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://bga.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://isq.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://umn.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://fja.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://qei.pengpengdd.cyou

[G13] 判断对象类型
来源：http://fdc.tarul.cn

Py:   isinstance(u, User)
来源：http://wvy.316326.xyz

PHP:  $u instanceof User
来源：http://wcy.yfazqb.com

JS:   u instanceof User
来源：http://yqg.iojbl.cn

TS:   u instanceof User
来源：http://mfc.ydjk.org.cn

Java: u instanceof User
来源：http://ukk.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jjv.daria6918.cn

Ruby: u.is_a?(User)
来源：http://bnh.kuanghao11.cn

C#:   u is User
来源：http://byb.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://sop.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uks.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://yaf.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tao.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://wca.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://lax.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://lgr.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lba.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://yss.sysykeji.top

[G15] 枚举
来源：http://duv.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qdr.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qbb.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kih.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xqq.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://wgr.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uwo.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://bhc.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nso.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://gxr.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tch.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://qtg.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://jic.sxryk.cn

TS:   Object.entries(obj)
来源：http://aoe.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qar.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xfl.fzhhl.top

Ruby: obj.instance_variables
来源：http://jqu.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://bzd.jqgfzy.top

================================================================================
来源：http://kkc.daxiang520.top

H. 异常与错误处理
来源：http://gtw.shanyushiyangtech.top

================================================================================
来源：http://gyv.jinqigfzy.top

[H01] try / catch 基础
来源：http://thz.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kcf.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pbr.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zpy.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vgz.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tei.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rkz.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jvj.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lcl.daxiang520.top

[H02] finally / ensure 收尾
来源：http://wxu.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kza.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qvs.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eag.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uvr.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://jnm.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jpc.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xeb.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lul.quarkkingdee.top

[H03] 主动抛出异常
来源：http://zmr.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://fyf.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://slj.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://mou.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://zgj.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sqc.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fil.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qme.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://czo.meibo888.top

[H04] 自定义异常类型
来源：http://ows.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://wuh.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ncz.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://raw.redwolf501.top

TS:   class MyError extends Error {}
来源：http://jiu.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://poj.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://loe.yj20258.top

Ruby: class MyError < StandardError; end
来源：http://bxl.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://zco.hcnkem.com

[H05] 捕获特定类型
来源：http://bci.shzxlz.cn

Py:   except ValueError as e:
来源：http://phw.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mxl.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://bwy.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://vgc.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://wyr.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sdg.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://xqf.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ney.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://ywl.uphjek.com

Py:   value = d.get("k") or default
来源：http://ddv.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qxx.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rgi.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zat.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tar.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ohx.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://hkk.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://dny.sjlbkw.cn

[H07] 断言
来源：http://ivt.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://zhk.zhixingplan.top

PHP:  assert($x > 0);
来源：http://pat.hesvh.cn

JS:   console.assert(x > 0);
来源：http://ddp.fzhhl.top

TS:   console.assert(x > 0);
来源：http://qwo.ybcxt.top

Java: assert x > 0 : "必须为正";
来源：http://jos.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sre.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pjn.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://yzp.0kj1m.cn

[H08] 获取错误信息与堆栈
来源：http://met.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://ffo.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mjw.daria6918.cn

JS:   e.message;  e.stack
来源：http://zjn.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bxw.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mhh.tanke756.top

Go:   err.Error()
来源：http://hvt.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://tln.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://pvr.yj20258.top

[H09] 带错误码的异常
来源：http://ibu.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://grb.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wvo.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vnp.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gtq.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uuc.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hjb.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://yde.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uba.zhoulong.xyz

[H10] 资源自动释放
来源：http://edb.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://zir.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xtd.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tgs.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xvn.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://byt.hysaishi.cn

Go:   defer f.Close()
来源：http://iok.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hen.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://num.jinyuanbaomall.cn

================================================================================
来源：http://yhz.bbcook.cn

I. 正则表达式
来源：http://hms.fehbvm.com

================================================================================
来源：http://ijv.yangfankeji.com

[I01] 判断是否匹配
来源：http://hes.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aab.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://pgf.cashguo.top

JS:   /\d+/.test(s)
来源：http://uth.ehwqpu.com

TS:   /\d+/.test(s)
来源：http://nra.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kyi.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsq.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://afp.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kzt.vqdsnc.cn

[I02] 提取所有匹配
来源：http://eeg.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://qyn.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sus.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://txl.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://cxl.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pih.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bsu.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://mgl.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xmp.haohaochexian.top

[I03] 提取捕获分组
来源：http://vzi.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xra.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ajm.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://krb.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xjv.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wqe.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://isl.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xwz.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lim.shangyingyoupin.top

[I04] 正则替换
来源：http://ato.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yqg.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sst.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://epc.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gwn.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://yco.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://seb.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kdx.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://usw.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://jvm.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://tog.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://njt.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://tcd.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://pac.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://gnx.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ooy.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://hud.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ewz.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dqt.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bho.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pjq.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pmn.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygr.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mmk.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rao.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bqw.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kgn.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://htu.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rjv.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mgt.fehbvm.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ogp.hesvh.cn

TS:   /error/gim
来源：http://jts.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vob.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pgu.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://ner.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gkr.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://gfh.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nxe.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xjk.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mis.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ruj.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uvo.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qfi.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://afb.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ttd.ydjk.org.cn

================================================================================
来源：http://abi.jlsjyb.cn

J. 日期与时间
来源：http://apl.tarul.cn

================================================================================
来源：http://ume.andypj.xyz

[J01] 获取当前时间
来源：http://dqw.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nyh.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qov.wangdashe.top

JS:   new Date();  Date.now()
来源：http://mxh.sysykeji.top

TS:   new Date();  Date.now()
来源：http://vfv.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jsu.meibo888.top

Go:   time.Now()
来源：http://urb.daxiang520.top

Ruby: Time.now
来源：http://diw.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pgs.jianghu66.top

[J02] 格式化输出
来源：http://sjy.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rya.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://taj.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xeq.uphjek.com

TS:   d.toISOString()
来源：http://buf.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bxy.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://plk.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hwq.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://akd.tian-w.cn

[J03] 字符串解析为日期
来源：http://lor.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wdl.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://alt.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://nod.redwolf501.top


<!-- 参考信息 -->