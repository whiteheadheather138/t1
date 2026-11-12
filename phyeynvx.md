代发 wailian999

Py:   class Admin(User): pass
来源：http://mcv.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://gst.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://rir.aizwys.cn

TS:   class Admin extends User {}
来源：http://brw.yanxiufei.cn

Java: class Admin extends User {}
来源：http://ucn.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aiq.zdqjudy.top

Ruby: class Admin < User; end
来源：http://gtd.ydzc1.top

C#:   class Admin : User {}
来源：http://ujb.quarkkingdee.top

[G06] 重写方法
来源：http://zqi.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://yvn.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vpx.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://rce.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://pwt.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://xir.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pqb.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://ity.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://uvk.yongpay.top

[G07] 调用父类方法
来源：http://qvs.redwolf501.top

Py:   super().greet()
来源：http://uxj.nanxuanxn.top

PHP:  parent::greet();
来源：http://dkk.tianlin.xyz

JS:   super.greet();
来源：http://ddi.meibo888.top

TS:   super.greet();
来源：http://mfz.bbcook.cn

Java: super.greet();
来源：http://xri.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fvg.cqqwz.cn

Ruby: super
来源：http://cps.hysaishi.cn

C#:   base.Greet();
来源：http://gin.quarkkingdee.top

[G08] 静态方法与属性
来源：http://vfs.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lms.9152youxi.cn

PHP:  public static function f() {}
来源：http://hyy.yonumen.top

JS:   static f() {}
来源：http://wbv.shangyingyoupin.top

TS:   static f(): void {}
来源：http://glh.ydzc1.top

Java: static void f() {}
来源：http://gbm.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mqv.vehdjk.com

Ruby: def self.f; end
来源：http://psh.sjlbkw.cn

C#:   public static void F() {}
来源：http://vgf.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://mhp.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://hgv.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://nhp.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://exy.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://grk.ywan-chungtsiang.top

Java: interface Shape { double area(); }
来源：http://rnx.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://sls.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nxp.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://irl.birdmap.top

[G10] 访问控制
来源：http://qtm.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://ili.yonumen.top

PHP:  public / protected / private
来源：http://nbv.yj20258888.top

JS:   #private 字段；其余公开
来源：http://iwq.hcnkem.com

TS:   public / protected / private
来源：http://hxx.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://cfi.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ipt.aizwys.cn

Ruby: public / protected / private
来源：http://ikv.iojbl.cn

C#:   public / protected / private / internal
来源：http://yaa.pycfn.com

[G11] getter / setter
来源：http://ouv.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://zby.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ahr.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://ibg.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://vmo.yonumen.top

Java: public String getName() { return name; }
来源：http://jwj.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://edt.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://ekw.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://auo.shangyingyoupin.top

[G12] 对象转字符串
来源：http://qar.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://ezh.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rly.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://zve.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://sro.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://iqx.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wck.havefunace.top

Ruby: def to_s; @name; end
来源：http://kyp.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://cmk.cucudq.cn

[G13] 判断对象类型
来源：http://rja.zdbjq.cn

Py:   isinstance(u, User)
来源：http://pnl.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://yga.gaohongyu789.top

JS:   u instanceof User
来源：http://iri.sysykeji.top

TS:   u instanceof User
来源：http://hof.xuanzx.com

Java: u instanceof User
来源：http://zzj.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dpo.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://xds.hysaishi.cn

C#:   u is User
来源：http://qyc.zhijiandao.cn

[G14] 数据类 / record
来源：http://lpr.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ijg.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://aqy.uphjek.com

JS:   // 无内置：普通类或对象字面量
来源：http://qoc.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://igb.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://skj.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://tkf.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dkk.birdmap.top

C#:   record User(string Name, int Age);
来源：http://eaq.daria6918.cn

[G15] 枚举
来源：http://hrw.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mps.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hxp.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nao.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nli.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://xxv.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fah.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://yrl.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iwm.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://ynk.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://spn.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://ulm.vehdjk.com

JS:   Object.entries(obj)
来源：http://zwx.yuxming.cn

TS:   Object.entries(obj)
来源：http://ajd.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ghk.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dew.guannengcc.top

Ruby: obj.instance_variables
来源：http://yjt.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://fre.andypj.xyz

================================================================================
来源：http://mzz.birdmap.top

H. 异常与错误处理
来源：http://imb.ehwqpu.com

================================================================================
来源：http://fnk.yj202588.top

[H01] try / catch 基础
来源：http://dya.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qtq.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gzg.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xeo.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rjf.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jcc.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kus.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dri.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://puc.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://voy.xuetiantiany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://thh.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://rkh.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nyj.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xgu.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ins.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nul.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ecc.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://esw.zdbjq.cn

[H03] 主动抛出异常
来源：http://cxh.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://hou.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vws.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://hsx.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://fzs.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nwx.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qyk.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://qab.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://pjz.wangdashe.top

[H04] 自定义异常类型
来源：http://rsr.316326.xyz

Py:   class MyError(Exception): pass
来源：http://xid.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://xch.sxryk.cn

JS:   class MyError extends Error {}
来源：http://cqa.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://mgb.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://iwz.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pvv.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://bcw.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://eti.sufxvd.cn

[H05] 捕获特定类型
来源：http://qzq.zhoulong.xyz

Py:   except ValueError as e:
来源：http://lwx.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://abk.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://yit.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://wou.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://tki.yongpay.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wfk.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://tgq.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bmv.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://lkb.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://jzz.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://pqt.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://zlx.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://epv.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hlb.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gqd.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://ksz.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://cdu.haohaochexian.top

[H07] 断言
来源：http://fuf.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://cuk.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://dbh.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://qui.bbcook.cn

TS:   console.assert(x > 0);
来源：http://lqy.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://wzx.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gzl.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tpk.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://yuv.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://hci.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://hau.sjlbkw.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mtk.tanke756.top

JS:   e.message;  e.stack
来源：http://mtg.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://fpt.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lxi.gaohongyu789.top

Go:   err.Error()
来源：http://krd.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://tsz.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://knt.hammf.cn

[H09] 带错误码的异常
来源：http://lnv.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ryl.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pkk.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://alw.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fqy.cdnleiting.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://csq.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tqc.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://rdy.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kwl.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://bth.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gtt.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ilt.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wia.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rdq.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xpg.sysykeji.top

Go:   defer f.Close()
来源：http://lpr.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://koz.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mtj.fktsv.cn

================================================================================
来源：http://dps.gogol.net.cn

I. 正则表达式
来源：http://wdq.dashuyun.cn

================================================================================
来源：http://muq.xziqi.cn

[I01] 判断是否匹配
来源：http://uyp.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wky.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://jno.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://uyd.mhx1999.top

TS:   /\d+/.test(s)
来源：http://evy.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fmg.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xjq.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://kfb.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pqs.tanke756.top

[I02] 提取所有匹配
来源：http://mgk.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://vuk.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ybf.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://czt.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://oww.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cru.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rzq.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://soa.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baq.xinyue.icu

[I03] 提取捕获分组
来源：http://pvi.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qqy.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mje.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sbd.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://spu.gzhubu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zjf.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qoh.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fob.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yvu.ctjpmb.com

[I04] 正则替换
来源：http://kfy.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://xqg.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ohg.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://skv.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://hyl.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://itz.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hjn.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ygu.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hgk.hnqzz.top

[I05] 按正则拆分
来源：http://nbt.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://hnb.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://alp.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://ech.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://dol.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://zbi.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lut.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://tqi.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jyq.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wvx.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ugr.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tna.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bta.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://osk.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jwu.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ste.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yhu.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fwf.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://yot.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://htw.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bfp.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://skk.jinqigfzy.top

TS:   /error/gim
来源：http://ifj.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qfa.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hjf.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://lof.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jct.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://nip.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dkb.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hwj.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qfv.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hdi.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://izd.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mpq.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fqf.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hzf.aibaodan.cn

================================================================================
来源：http://upk.birdmap.top

J. 日期与时间
来源：http://vyb.sweek.top

================================================================================
来源：http://umw.chenjidiqi.icu

[J01] 获取当前时间
来源：http://lkr.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bxs.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://msx.xuanzx.com

JS:   new Date();  Date.now()
来源：http://vzn.yj202588.top

TS:   new Date();  Date.now()
来源：http://mie.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wqx.ehwqpu.com

Go:   time.Now()
来源：http://qqc.sxryk.cn

Ruby: Time.now
来源：http://pnu.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mmi.zhengqikj.top

[J02] 格式化输出
来源：http://awq.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fbb.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bkg.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dqy.nanxuanxn.top

TS:   d.toISOString()
来源：http://kuw.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hhf.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aql.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://atw.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vlg.mhx1999.top

[J03] 字符串解析为日期
来源：http://ybz.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hhi.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bky.yj20258.top

JS:   new Date("2024-01-02")
来源：http://sfg.meibo888.top


<!-- 参考信息 -->