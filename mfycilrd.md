代发 wailian999

Ruby: @name = "x"
来源：http://mci.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://hwb.bbcook.cn

[G04] 定义方法
来源：http://qwa.pycfn.com

Py:   def greet(self): return self.name
来源：http://edq.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rhx.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://zxe.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://blq.chenzaomai.com

Java: String greet() { return name; }
来源：http://yiw.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sfq.haohaochexian.top

Ruby: def greet; @name; end
来源：http://gha.bjfxy.top

C#:   public string Greet() => Name;
来源：http://fsk.ywan-chungtsiang.top

[G05] 继承
来源：http://xuo.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://fdp.fengsongda.top

PHP:  class Admin extends User {}
来源：http://viu.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://oxq.quarkkingdee.top

TS:   class Admin extends User {}
来源：http://nsw.jianghu66.top

Java: class Admin extends User {}
来源：http://nkz.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yck.52xcode.cn

Ruby: class Admin < User; end
来源：http://cql.shzxlz.cn

C#:   class Admin : User {}
来源：http://bbo.mhx1999.top

[G06] 重写方法
来源：http://pyz.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://sjc.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lke.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://bwk.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://tyf.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://zoi.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://owh.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://gzr.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://xny.jyoumei.cn

[G07] 调用父类方法
来源：http://tlp.shzxlz.cn

Py:   super().greet()
来源：http://oet.sjlbkw.cn

PHP:  parent::greet();
来源：http://wjv.jinqigufen.top

JS:   super.greet();
来源：http://xdi.quarkkingdee.top

TS:   super.greet();
来源：http://tnr.9152youxi.cn

Java: super.greet();
来源：http://qqm.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sfv.hysaishi.cn

Ruby: super
来源：http://khy.hfpthk.cn

C#:   base.Greet();
来源：http://feb.gotoacloud.top

[G08] 静态方法与属性
来源：http://tae.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://esg.sxryk.cn

PHP:  public static function f() {}
来源：http://mky.fktsv.cn

JS:   static f() {}
来源：http://pdc.mhx1999.top

TS:   static f(): void {}
来源：http://qnh.yangfankeji.com

Java: static void f() {}
来源：http://afy.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tgv.ivvv.top

Ruby: def self.f; end
来源：http://fbx.fktsv.cn

C#:   public static void F() {}
来源：http://aut.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://mzy.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://uxc.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zrv.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://alu.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://izi.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://kbu.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://cba.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rnf.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://yme.tarul.cn

[G10] 访问控制
来源：http://khf.9152youxi.cn

Py:   约定 _protected / __private（不强制）
来源：http://jki.cashguo.top

PHP:  public / protected / private
来源：http://brj.c1oappe.top

JS:   #private 字段；其余公开
来源：http://nqe.zhijiandao.cn

TS:   public / protected / private
来源：http://vvj.cashguo.top

Java: public / protected / private / 默认包级
来源：http://czx.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nqh.chenjidiqi.icu

Ruby: public / protected / private
来源：http://woy.snrcjt.cn

C#:   public / protected / private / internal
来源：http://kqa.yj20258888.top

[G11] getter / setter
来源：http://wek.yueranfly.top

Py:   @property 与 @x.setter
来源：http://njg.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ovw.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://ypt.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://ses.haohaochexian.top

Java: public String getName() { return name; }
来源：http://awc.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ktd.hnqzz.top

Ruby: attr_accessor :name
来源：http://kmz.xziqi.cn

C#:   public string Name { get; set; }
来源：http://vtr.daria6918.cn

[G12] 对象转字符串
来源：http://bcy.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://hgf.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dun.redwolf501.top

JS:   toString() { return this.name; }
来源：http://xhc.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://oru.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://pqb.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://knv.zhiwuduotai.top

Ruby: def to_s; @name; end
来源：http://ooo.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://sme.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://hyl.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://aaj.havefunace.top

PHP:  $u instanceof User
来源：http://oti.pengpengdd.cyou

JS:   u instanceof User
来源：http://rwy.jinqigufen.top

TS:   u instanceof User
来源：http://bhn.daxiang520.top

Java: u instanceof User
来源：http://ozx.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://osf.wangdashe.top

Ruby: u.is_a?(User)
来源：http://lcy.cdnleiting.top

C#:   u is User
来源：http://bnq.kuanghao11.cn

[G14] 数据类 / record
来源：http://zys.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hav.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://kne.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://vqa.yongpay.top

TS:   type User = { name: string; age: number };
来源：http://eov.jinyuanbaomall.cn

Java: record User(String name, int age) {}
来源：http://gwz.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://dtd.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ipt.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://lae.zhijiandao.cn

[G15] 枚举
来源：http://lna.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zfw.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://nnc.hywenlv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wxs.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qsw.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://jjq.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uji.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://mti.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://alg.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://wgp.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbo.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://vsm.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://dhq.jiagoushi.top

TS:   Object.entries(obj)
来源：http://uus.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ivh.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://tfs.tian-w.cn

Ruby: obj.instance_variables
来源：http://jwg.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://iso.ivvv.top

================================================================================
来源：http://bnh.0kj1m.cn

H. 异常与错误处理
来源：http://sax.52xcode.cn

================================================================================
来源：http://xep.ehwqpu.com

[H01] try / catch 基础
来源：http://pks.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gdw.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nfv.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vzm.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cah.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nkb.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sdl.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kco.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yfp.nwbrower.top

[H02] finally / ensure 收尾
来源：http://qss.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oho.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ode.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ijq.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xzu.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://uqw.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://thp.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://seu.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zko.vehdjk.com

[H03] 主动抛出异常
来源：http://ywq.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://cyb.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://slp.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://xuv.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://tlv.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ved.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dxi.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zup.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qip.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://tph.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://htn.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ywb.havefunace.top

JS:   class MyError extends Error {}
来源：http://qif.birdmap.top

TS:   class MyError extends Error {}
来源：http://zgw.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://cfv.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ebx.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://dfy.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://mav.snrcjt.cn

[H05] 捕获特定类型
来源：http://fhb.bbcook.cn

Py:   except ValueError as e:
来源：http://reo.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jpt.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://mje.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://uct.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://xgt.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ezn.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://rqf.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wbc.gzhubu.top

[H06] 可选值 / 空值安全访问
来源：http://ewt.yj202588.top

Py:   value = d.get("k") or default
来源：http://hzw.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bgx.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bkg.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://ijv.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://goj.ydjk.org.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lsm.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://guw.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://kss.wangshuangyany.cn

[H07] 断言
来源：http://rpi.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://ixo.xylfe.cn

PHP:  assert($x > 0);
来源：http://hfs.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://oua.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://amk.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://qmi.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hqf.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://byj.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://jeh.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://qkd.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://tct.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://boz.fehbvm.com

JS:   e.message;  e.stack
来源：http://qmv.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://oox.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://bgi.vqdsnc.cn

Go:   err.Error()
来源：http://nge.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://rms.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://rfk.cdnleiting.top

[H09] 带错误码的异常
来源：http://kqm.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rmp.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cms.guowangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rzc.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lxt.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://frb.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kox.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://tko.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://hth.dianchejie.cn

[H10] 资源自动释放
来源：http://ytw.jinqigufen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dga.gogol.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bgs.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nym.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rzo.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ktu.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://dcy.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hah.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qou.gotoacloud.top

================================================================================
来源：http://nci.zdbjq.cn

I. 正则表达式
来源：http://llb.cdnleiting.top

================================================================================
来源：http://sfz.tanke756.top

[I01] 判断是否匹配
来源：http://ygw.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jvc.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://qil.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://mpd.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://bey.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dwk.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ocz.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://ukq.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uuz.gogol.net.cn

[I02] 提取所有匹配
来源：http://jwg.redwolf501.top

Py:   re.findall(r"\d+", s)
来源：http://pzg.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xre.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xni.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://qyd.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yap.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qfi.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://iaj.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jum.gogol.net.cn

[I03] 提取捕获分组
来源：http://msc.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://orh.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wwo.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xxb.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vdw.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://heu.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lkw.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ftn.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qsp.sufxvd.cn

[I04] 正则替换
来源：http://wpk.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gwd.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lkq.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gdd.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rue.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://vfr.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://fhr.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bpg.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uxy.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://lcm.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xhb.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aly.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://quv.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://nel.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://zqo.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://woo.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://vjg.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://grt.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ffs.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bmj.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pfz.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xrs.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ymj.fengsongda.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ggf.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gme.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixo.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rqz.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://mgj.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cba.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://slj.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://onv.ywan-chungtsiang.top

TS:   /error/gim
来源：http://dhr.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zsy.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mka.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://ocy.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qrs.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://eru.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fet.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zoy.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qgu.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dgs.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vdk.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qmd.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gcf.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yzj.iojbl.cn

================================================================================
来源：http://wbf.ppjwa.cn

J. 日期与时间
来源：http://fav.shzxlz.cn

================================================================================
来源：http://lmb.sjlbkw.cn

[J01] 获取当前时间
来源：http://wpv.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cbk.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sdd.uphjek.com

JS:   new Date();  Date.now()
来源：http://ygz.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://zwz.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://wfj.jinqigufen.top

Go:   time.Now()
来源：http://odt.jlsjyb.cn

Ruby: Time.now
来源：http://ydw.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pvl.jianghu66.top

[J02] 格式化输出
来源：http://pca.daria6918.cn


<!-- 参考信息 -->