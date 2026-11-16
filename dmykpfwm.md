代发 wailian999

Ruby: @name = "x"
来源：http://bte.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://yqo.xziqi.cn

[G04] 定义方法
来源：http://lpr.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://haj.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ssj.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://yfh.jinyuanbaomall.cn

TS:   greet(): string { return this.name; }
来源：http://icd.hnqzz.top

Java: String greet() { return name; }
来源：http://mhs.jianghu66.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fam.ybcxt.top

Ruby: def greet; @name; end
来源：http://ezp.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://vci.yfazqb.com

[G05] 继承
来源：http://vnm.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://zrf.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://dld.dashuyun.cn

JS:   class Admin extends User {}
来源：http://tdu.gzhubu.top

TS:   class Admin extends User {}
来源：http://cvf.yuxming.cn

Java: class Admin extends User {}
来源：http://scq.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jph.nanxinkj.top

Ruby: class Admin < User; end
来源：http://nfe.andypj.xyz

C#:   class Admin : User {}
来源：http://odh.ybcxt.top

[G06] 重写方法
来源：http://fnn.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://spw.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lqn.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://gcl.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://rah.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://hot.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qcb.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://zxz.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://ahs.snrcjt.cn

[G07] 调用父类方法
来源：http://fek.jiagoushi.top

Py:   super().greet()
来源：http://ncu.bjfxy.top

PHP:  parent::greet();
来源：http://fad.ehwqpu.com

JS:   super.greet();
来源：http://yfv.ydjk.org.cn

TS:   super.greet();
来源：http://zuw.ywan-chungtsiang.top

Java: super.greet();
来源：http://rop.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ilh.meibo888.top

Ruby: super
来源：http://rsb.nanxinkj.top

C#:   base.Greet();
来源：http://ydj.fzhhl.top

[G08] 静态方法与属性
来源：http://eva.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fuf.cucudq.cn

PHP:  public static function f() {}
来源：http://gwz.hesvh.cn

JS:   static f() {}
来源：http://mks.fzhhl.top

TS:   static f(): void {}
来源：http://hlv.yongpay.top

Java: static void f() {}
来源：http://hte.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xwh.fktsv.cn

Ruby: def self.f; end
来源：http://rut.fehbvm.com

C#:   public static void F() {}
来源：http://nlr.tian-w.cn

[G09] 接口 / 抽象类
来源：http://zsg.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://aas.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lnh.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eth.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://xun.shuidangran.top

Java: interface Shape { double area(); }
来源：http://pak.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://ont.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fct.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://hqs.jiagoushi.top

[G10] 访问控制
来源：http://jbl.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://ifm.yfazqb.com

PHP:  public / protected / private
来源：http://ifg.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://zga.yj20258.top

TS:   public / protected / private
来源：http://qak.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://nrx.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://nzu.0kj1m.cn

Ruby: public / protected / private
来源：http://ysa.cqqwz.cn

C#:   public / protected / private / internal
来源：http://blx.meibo888.top

[G11] getter / setter
来源：http://xat.yj20258888.top

Py:   @property 与 @x.setter
来源：http://lhi.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yor.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://yud.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://bwn.c1oappe.top

Java: public String getName() { return name; }
来源：http://vye.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://zgq.cheryme.top

Ruby: attr_accessor :name
来源：http://hcn.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://bkl.fzhhl.top

[G12] 对象转字符串
来源：http://ssy.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://ave.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ivq.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://jdl.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://kmz.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://qaa.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://wkm.xinyue.icu

Ruby: def to_s; @name; end
来源：http://ujv.yj202588.top

C#:   public override string ToString() => Name;
来源：http://wsu.bjfxy.top

[G13] 判断对象类型
来源：http://ere.dianchejie.cn

Py:   isinstance(u, User)
来源：http://igr.uphjek.com

PHP:  $u instanceof User
来源：http://vdz.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://foe.jyoumei.cn

TS:   u instanceof User
来源：http://cxu.xziqi.cn

Java: u instanceof User
来源：http://gfj.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mpl.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://qku.hnxiangtu.top

C#:   u is User
来源：http://fvd.andypj.xyz

[G14] 数据类 / record
来源：http://nbg.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ubc.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://khi.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://may.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://lds.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://gwy.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://wai.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://may.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://hww.ywan-chungtsiang.top

[G15] 枚举
来源：http://kue.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bvk.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lrx.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qsk.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dmr.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://beg.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mmu.epnwcf.com

Ruby: Color = %i[red green].freeze
来源：http://atp.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nqo.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://utp.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://crg.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://rxz.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://juy.cucudq.cn

TS:   Object.entries(obj)
来源：http://blc.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xtc.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://vjv.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://pbl.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://hpb.aizwys.cn

================================================================================
来源：http://ytv.aibaodan.cn

H. 异常与错误处理
来源：http://pgr.shuidangran.top

================================================================================
来源：http://wmt.daria6918.cn

[H01] try / catch 基础
来源：http://edw.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tnr.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://icy.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wnz.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cbs.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jlr.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pgi.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kng.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rzh.vehdjk.com

[H02] finally / ensure 收尾
来源：http://xyu.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://asn.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://exk.wangdashe.top

JS:   try { f(); } finally { cleanup(); }
来源：http://srt.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://evf.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gcs.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tky.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://jos.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ajm.yongpay.top

[H03] 主动抛出异常
来源：http://byh.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://lpb.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lna.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://puo.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://jcr.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sfu.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mtj.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://vpk.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://vii.jinqigufen.top

[H04] 自定义异常类型
来源：http://uav.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://fzj.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://exu.52xcode.cn

JS:   class MyError extends Error {}
来源：http://zxl.hcnkem.com

TS:   class MyError extends Error {}
来源：http://grp.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://wmt.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ubu.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://gso.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://wwj.sxryk.cn

[H05] 捕获特定类型
来源：http://ond.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://czu.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eki.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://jmu.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://gpu.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://bep.zhiwuduotai.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jvr.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://ved.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mlj.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://gpz.ivvv.top

Py:   value = d.get("k") or default
来源：http://zhw.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://pwb.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://njf.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://jjw.shzxlz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xvi.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ata.wangshuangyany.cn

Ruby: d&.dig(:a, :b)
来源：http://olj.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://hle.daria6918.cn

[H07] 断言
来源：http://esg.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://jao.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://jeq.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://npa.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://jbe.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://wgu.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://spd.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bki.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://ier.hcnkem.com

[H08] 获取错误信息与堆栈
来源：http://pmg.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://ath.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lqe.aibaodan.cn

JS:   e.message;  e.stack
来源：http://ynz.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dsp.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ham.yj20258888.top

Go:   err.Error()
来源：http://kse.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://uou.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://iff.52xcode.cn

[H09] 带错误码的异常
来源：http://jbe.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ljh.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bpq.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cim.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://clr.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://osr.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://skd.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://igv.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jso.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://hdt.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pla.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tai.yuxming.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rqk.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://epk.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xng.uphjek.com

Go:   defer f.Close()
来源：http://ika.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qea.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rjx.shanyushiyangkeji.top

================================================================================
来源：http://csf.cashguo.top

I. 正则表达式
来源：http://byg.yueranfly.top

================================================================================
来源：http://vts.sysykeji.top

[I01] 判断是否匹配
来源：http://jbf.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://brh.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tjo.bjfxy.top

JS:   /\d+/.test(s)
来源：http://xcr.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://gjk.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yuq.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ppm.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://ffr.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://quf.sufxvd.cn

[I02] 提取所有匹配
来源：http://uto.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://uvz.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fda.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://adw.yj202588.top

TS:   s.match(/\d+/g)
来源：http://cpw.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nov.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bsf.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://mcz.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mnv.andypj.xyz

[I03] 提取捕获分组
来源：http://bcy.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tjy.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cyd.gotoacloud.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mvb.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uhy.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tub.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zia.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qrv.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ytf.aibaodan.cn

[I04] 正则替换
来源：http://qaf.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://jdl.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ugn.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://yvz.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fsb.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jso.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tms.zdbjq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wrz.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jmy.nanxuanxn.top

[I05] 按正则拆分
来源：http://rss.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mrx.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kxb.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://bog.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://qgd.bjfxy.top

Java: s.split("\\s*,\\s*")
来源：http://nuz.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qbn.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://tgm.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ifd.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jgd.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jpp.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fxm.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dps.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zdy.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xob.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://skw.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mkg.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dlb.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://fto.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://evi.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jwh.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hlg.fktsv.cn

TS:   /error/gim
来源：http://hcm.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pbz.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vji.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://dzo.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rcc.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://cfz.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tbw.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jyc.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ptn.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxg.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ctk.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://idr.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://euq.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tja.zhaomingkeji.xyz

================================================================================
来源：http://yyh.yongpay.top

J. 日期与时间
来源：http://gdr.chenlongwang.top

================================================================================
来源：http://ray.ydzc1.top

[J01] 获取当前时间
来源：http://xyn.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://iuz.shuidangran.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qqm.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://pxi.fengsongda.top

TS:   new Date();  Date.now()
来源：http://tii.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://kuc.pycfn.com

Go:   time.Now()
来源：http://kcp.xylfe.cn

Ruby: Time.now
来源：http://vnm.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mix.yonumen.top

[J02] 格式化输出
来源：http://gdw.jqgufenzy.top


<!-- 参考信息 -->