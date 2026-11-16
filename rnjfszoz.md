代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://cbg.havefunace.top

[G03] 实例属性
来源：http://bae.52xcode.cn

Py:   self.name = "x"
来源：http://wsy.daria6918.cn

PHP:  public string $name = "x";
来源：http://wve.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://tjq.vqdsnc.cn

TS:   name: string = "x";
来源：http://ogn.kuanghao11.cn

Java: private String name;
来源：http://jdb.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dgc.fktsv.cn

Ruby: @name = "x"
来源：http://ene.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://uvr.shuidangran.top

[G04] 定义方法
来源：http://wfh.quarkkingdee.top

Py:   def greet(self): return self.name
来源：http://ckr.hesvh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hiq.yj20258888.top

JS:   greet() { return this.name; }
来源：http://iuv.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://cap.nanxuanxn.top

Java: String greet() { return name; }
来源：http://rbt.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vhm.xylfe.cn

Ruby: def greet; @name; end
来源：http://rse.sysykeji.top

C#:   public string Greet() => Name;
来源：http://rqq.sxryk.cn

[G05] 继承
来源：http://xnm.xuanzx.com

Py:   class Admin(User): pass
来源：http://dby.meibo888.top

PHP:  class Admin extends User {}
来源：http://nup.daxiang520.top

JS:   class Admin extends User {}
来源：http://rsd.sxryk.cn

TS:   class Admin extends User {}
来源：http://kck.sxryk.cn

Java: class Admin extends User {}
来源：http://zii.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hep.uphjek.com

Ruby: class Admin < User; end
来源：http://veo.xziqi.cn

C#:   class Admin : User {}
来源：http://isj.haohaochexian.top

[G06] 重写方法
来源：http://nfn.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://zwp.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qrh.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://aia.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://qks.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://ttw.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://szo.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://quw.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://lxp.yangfankeji.com

[G07] 调用父类方法
来源：http://rie.chenzaomai.com

Py:   super().greet()
来源：http://uny.ivvv.top

PHP:  parent::greet();
来源：http://bwm.yfazqb.com

JS:   super.greet();
来源：http://zpi.jinyuanbaomall.cn

TS:   super.greet();
来源：http://bof.shangyingyoupin.top

Java: super.greet();
来源：http://wyc.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zmk.andypj.xyz

Ruby: super
来源：http://uvp.wangshuangyany.cn

C#:   base.Greet();
来源：http://prx.tian-w.cn

[G08] 静态方法与属性
来源：http://ehv.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://azj.gogol.net.cn

PHP:  public static function f() {}
来源：http://mzu.yueranfly.top

JS:   static f() {}
来源：http://mcd.cdnleiting.top

TS:   static f(): void {}
来源：http://snk.gogol.net.cn

Java: static void f() {}
来源：http://hug.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zef.nanxuanxn.top

Ruby: def self.f; end
来源：http://qcm.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://efz.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://lfu.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://klv.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://cvs.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://jzw.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://doe.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://etk.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ucy.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://frq.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://pxb.guowangkeji.top

[G10] 访问控制
来源：http://fwb.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://kjc.yangfankeji.com

PHP:  public / protected / private
来源：http://dls.c1oappe.top

JS:   #private 字段；其余公开
来源：http://xen.nwbrower.top

TS:   public / protected / private
来源：http://mtj.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://rns.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wnt.daria6918.cn

Ruby: public / protected / private
来源：http://ohm.tianlin.xyz

C#:   public / protected / private / internal
来源：http://dnk.tarul.cn

[G11] getter / setter
来源：http://ssk.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://qdx.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oqf.birdmap.top

JS:   get name() { return this._name; }
来源：http://lul.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://uoz.sufxvd.cn

Java: public String getName() { return name; }
来源：http://rru.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nob.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://rbp.yfazqb.com

C#:   public string Name { get; set; }
来源：http://upj.shangyingyoupin.top

[G12] 对象转字符串
来源：http://ctn.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://syt.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://scp.sxryk.cn

JS:   toString() { return this.name; }
来源：http://eqn.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://adt.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://wss.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://ual.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://saz.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://ebw.gaohongyu789.top

[G13] 判断对象类型
来源：http://udo.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://dkf.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://vxj.pycfn.com

JS:   u instanceof User
来源：http://dvo.pengpengdd.cyou

TS:   u instanceof User
来源：http://klx.bbcook.cn

Java: u instanceof User
来源：http://hfu.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://akg.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://tcl.cheryme.top

C#:   u is User
来源：http://yrx.hnxiangtu.top

[G14] 数据类 / record
来源：http://xig.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yav.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://tcp.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://stk.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://god.xinyue.icu

Java: record User(String name, int age) {}
来源：http://ufw.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://gjt.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dsc.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://ijz.yj202588.top

[G15] 枚举
来源：http://prm.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gxq.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gvo.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ekb.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qlk.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://zwn.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dfv.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://czw.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://evh.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://mlq.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nwc.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://ymk.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://ffx.vehdjk.com

TS:   Object.entries(obj)
来源：http://mxl.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gfp.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ekb.yongpay.top

Ruby: obj.instance_variables
来源：http://yoe.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://klr.tanke756.top

================================================================================
来源：http://nmo.sysykeji.top

H. 异常与错误处理
来源：http://ovd.yanxiufei.cn

================================================================================
来源：http://qqg.andypj.xyz

[H01] try / catch 基础
来源：http://vfn.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kim.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xmn.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://euq.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cvf.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yxm.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qiz.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jol.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uih.zhoulong.xyz

[H02] finally / ensure 收尾
来源：http://nda.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://xsx.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cyf.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vfu.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://jhd.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wxj.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://unp.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xtl.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jdu.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://kwc.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://vkb.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rln.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://ijn.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://rqb.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://jxg.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kpm.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hvu.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://pye.ctjpmb.com

[H04] 自定义异常类型
来源：http://vcu.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://crk.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://yrz.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://ave.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://sqd.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://hsl.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ksg.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://bry.mhx1999.top

C#:   class MyException : Exception {}
来源：http://ewc.jinqigufen.top

[H05] 捕获特定类型
来源：http://lxd.hywenlv.cn

Py:   except ValueError as e:
来源：http://vvw.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://afc.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://sgb.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://mdh.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://sce.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cbe.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://pth.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rqi.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://rjt.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://rng.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ekr.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ttl.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://wld.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gim.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sqn.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://roj.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://llo.52xcode.cn

[H07] 断言
来源：http://gov.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://dur.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://roo.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://zci.sxryk.cn

TS:   console.assert(x > 0);
来源：http://jua.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://dom.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sex.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://oda.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://agd.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://pet.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://tby.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rtl.zdbjq.cn

JS:   e.message;  e.stack
来源：http://dsy.ybcxt.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jvh.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mbz.nanxuanxn.top

Go:   err.Error()
来源：http://rri.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://rwz.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://hlx.jianghu66.top

[H09] 带错误码的异常
来源：http://mxo.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wze.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tog.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://shy.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dvs.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xkq.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tjj.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lqg.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ska.jyoumei.cn

[H10] 资源自动释放
来源：http://sgb.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jzi.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lhh.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xhd.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tkh.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gcg.xylfe.cn

Go:   defer f.Close()
来源：http://eng.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kra.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://grq.meibo888.top

================================================================================
来源：http://ege.shangyingyoupin.top

I. 正则表达式
来源：http://kbw.xinyue.icu

================================================================================
来源：http://gvk.cashguo.top

[I01] 判断是否匹配
来源：http://ore.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lqs.xingfuxueyuan.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://vfc.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://zng.hcnkem.com

TS:   /\d+/.test(s)
来源：http://gsz.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xdy.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsn.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://hqq.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://frf.uphjek.com

[I02] 提取所有匹配
来源：http://ies.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://fco.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wdw.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xxx.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://lfm.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tld.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ryt.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://kwi.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ext.jqgufenzy.top

[I03] 提取捕获分组
来源：http://jks.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ulb.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yqr.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iir.jinghuilouyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tev.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ebq.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hoy.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cbl.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ejy.yuanzhike.top

[I04] 正则替换
来源：http://dck.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nbh.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ovm.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://ezl.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://kql.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://uac.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ple.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mqx.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://deg.shangyingyoupin.top

[I05] 按正则拆分
来源：http://yrc.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://gak.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yco.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://soh.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://uif.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://gub.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bog.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://ylh.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yur.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oyu.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uzt.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mnj.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iuz.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfx.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bll.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zqt.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yjp.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zav.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://opc.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sym.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://opx.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yis.316326.xyz

TS:   /error/gim
来源：http://inv.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xqb.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vqd.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://wzl.snrcjt.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vro.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://zef.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tno.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dqz.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://frc.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pbz.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xlw.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://adw.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zrr.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jcn.hammf.cn

================================================================================
来源：http://xla.vehdjk.com

J. 日期与时间
来源：http://euc.shzxlz.cn

================================================================================
来源：http://bjx.zdqjudy.top

[J01] 获取当前时间
来源：http://iml.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ctv.zhixingplan.top


<!-- 参考信息 -->