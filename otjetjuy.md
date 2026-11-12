代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://uyn.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://eav.havefunace.top

C#:   public string Greet() => Name;
来源：http://axp.daxiang520.top

[G05] 继承
来源：http://ltz.xylfe.cn

Py:   class Admin(User): pass
来源：http://aon.yj20258.top

PHP:  class Admin extends User {}
来源：http://yay.tian-w.cn

JS:   class Admin extends User {}
来源：http://hkj.svipenyu.cn

TS:   class Admin extends User {}
来源：http://uzp.fengsongda.top

Java: class Admin extends User {}
来源：http://mbz.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rno.bbcook.cn

Ruby: class Admin < User; end
来源：http://jaw.zhixingplan.top

C#:   class Admin : User {}
来源：http://pbb.sufxvd.cn

[G06] 重写方法
来源：http://lsv.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://qhr.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://imf.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://urt.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://mtt.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://mhy.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jhl.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://nyn.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://iws.hcnkem.com

[G07] 调用父类方法
来源：http://zvs.tian-w.cn

Py:   super().greet()
来源：http://xhi.ctjpmb.com

PHP:  parent::greet();
来源：http://vmp.fehbvm.com

JS:   super.greet();
来源：http://dvx.sjlbkw.cn

TS:   super.greet();
来源：http://lcc.smart0.xyz

Java: super.greet();
来源：http://mvu.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ylk.xuanzx.com

Ruby: super
来源：http://npn.hammf.cn

C#:   base.Greet();
来源：http://rvu.xylfe.cn

[G08] 静态方法与属性
来源：http://wds.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lvg.daxiang520.top

PHP:  public static function f() {}
来源：http://lon.yangfankeji.com

JS:   static f() {}
来源：http://dwd.tianlin.xyz

TS:   static f(): void {}
来源：http://lbr.svipenyu.cn

Java: static void f() {}
来源：http://whg.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ifc.yuanzhike.top

Ruby: def self.f; end
来源：http://wzv.pengpengdd.cyou

C#:   public static void F() {}
来源：http://jxo.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://ijv.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://gby.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wgp.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nba.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://zqt.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://bnm.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://rrf.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gyv.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://dyd.sweek.top

[G10] 访问控制
来源：http://yod.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://fzg.pycfn.com

PHP:  public / protected / private
来源：http://gsz.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://csl.yuanzhike.top

TS:   public / protected / private
来源：http://tqb.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://frr.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jnh.zdqjudy.top

Ruby: public / protected / private
来源：http://sid.tianlin.xyz

C#:   public / protected / private / internal
来源：http://fcr.fzhhl.top

[G11] getter / setter
来源：http://zjv.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://gcs.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://psk.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://aog.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://mmz.andypj.xyz

Java: public String getName() { return name; }
来源：http://gpw.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lyj.hammf.cn

Ruby: attr_accessor :name
来源：http://ukr.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://hay.9152youxi.cn

[G12] 对象转字符串
来源：http://dnq.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://izn.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://hil.hcnkem.com

JS:   toString() { return this.name; }
来源：http://ija.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://knt.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://ijw.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uth.wangdashe.top

Ruby: def to_s; @name; end
来源：http://kkw.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://mxw.zhoulong.xyz

[G13] 判断对象类型
来源：http://qwy.jiagoushi.top

Py:   isinstance(u, User)
来源：http://dcn.aibaodan.cn

PHP:  $u instanceof User
来源：http://bjd.kuanghao11.cn

JS:   u instanceof User
来源：http://xok.zhijiandao.cn

TS:   u instanceof User
来源：http://qfs.zhixingplan.top

Java: u instanceof User
来源：http://uef.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jpq.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://rpt.jinghuilouyu.cn

C#:   u is User
来源：http://wlc.hcnkem.com

[G14] 数据类 / record
来源：http://dso.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kra.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://pzg.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://yuk.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://iot.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://jzg.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://mpc.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qmt.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://awp.9152youxi.cn

[G15] 枚举
来源：http://rkr.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sab.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cjp.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nsr.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jwt.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://wml.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lzk.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://ujs.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nhd.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://yls.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ahp.hammf.cn

PHP:  get_object_vars($obj);
来源：http://aai.ehwqpu.com

JS:   Object.entries(obj)
来源：http://ntl.tian-w.cn

TS:   Object.entries(obj)
来源：http://gtw.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yzm.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vrd.yfazqb.com

Ruby: obj.instance_variables
来源：http://zis.pengpengdd.cyou

C#:   // 用反射或 System.Text.Json
来源：http://sjm.kuanghao11.cn

================================================================================
来源：http://ndx.xuetiantiany.cn

H. 异常与错误处理
来源：http://pzk.yonumen.top

================================================================================
来源：http://tvf.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://lul.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iab.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eqv.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ttg.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://opu.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cwa.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://byt.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kps.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pkd.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://wgj.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://mrq.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://inq.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://wql.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://moy.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://pfa.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qwh.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://voz.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gpp.jqgfzy.top

[H03] 主动抛出异常
来源：http://oll.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://ggy.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zwk.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://uzv.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://wxs.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vay.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hxq.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qpv.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://szg.kuanghao11.cn

[H04] 自定义异常类型
来源：http://igx.hnqzz.top

Py:   class MyError(Exception): pass
来源：http://plu.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://puy.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://gsn.yj202588.top

TS:   class MyError extends Error {}
来源：http://uin.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://hxh.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sdh.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://mpd.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://pwg.ybcxt.top

[H05] 捕获特定类型
来源：http://ntk.nanxinkj.top

Py:   except ValueError as e:
来源：http://jqq.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pwf.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://egs.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://eec.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://eta.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zqp.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://zmq.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://heb.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://qfz.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://ciy.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://glc.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://ubk.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://nqs.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yxp.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mto.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://wtz.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://hvx.yueranfly.top

[H07] 断言
来源：http://vmq.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://qhb.hywenlv.cn

PHP:  assert($x > 0);
来源：http://mpe.uphjek.com

JS:   console.assert(x > 0);
来源：http://ipf.yj20258.top

TS:   console.assert(x > 0);
来源：http://qlv.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://kbj.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jcq.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iiy.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://ceu.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://gzh.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://zob.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hzh.aizwys.cn

JS:   e.message;  e.stack
来源：http://oqs.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://kzn.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pel.jinghuilouyu.cn

Go:   err.Error()
来源：http://oua.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://ehh.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://ugo.chenlongwang.top

[H09] 带错误码的异常
来源：http://gmq.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qyr.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://zlu.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lwa.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hwg.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hok.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ijl.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://beh.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cup.shuidangran.top

[H10] 资源自动释放
来源：http://vtv.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wub.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qss.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://soy.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vrv.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ueo.haohaochexian.top

Go:   defer f.Close()
来源：http://fgf.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mbr.shanyushiyangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jfc.jiagoushi.top

================================================================================
来源：http://cxo.bbcook.cn

I. 正则表达式
来源：http://rke.tianlin.xyz

================================================================================
来源：http://ofr.guannengcc.top

[I01] 判断是否匹配
来源：http://mhl.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fyi.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gbn.xinyue.icu

JS:   /\d+/.test(s)
来源：http://bbd.epnwcf.com

TS:   /\d+/.test(s)
来源：http://oox.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rvr.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zyo.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://oje.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uti.jinqigufen.top

[I02] 提取所有匹配
来源：http://xvh.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://qdn.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vvk.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dmj.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://ptg.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://avq.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wkb.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://hxa.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nrm.ybcxt.top

[I03] 提取捕获分组
来源：http://ndi.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://emf.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dxu.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://umn.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qxa.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://znw.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bdf.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bro.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oef.hfpthk.cn

[I04] 正则替换
来源：http://ryg.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eye.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qnc.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zui.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://wdl.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://tqf.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ksp.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rbd.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ywn.yj202588.top

[I05] 按正则拆分
来源：http://tfc.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://cql.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gwn.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://hte.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://qib.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://igo.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yge.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://fpk.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oab.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sgr.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zpz.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ual.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ash.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dhv.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kvj.yj202588.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://njp.cheryme.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zkd.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ubh.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://iim.iojbl.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qws.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://luh.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://izo.snrcjt.cn

TS:   /error/gim
来源：http://eld.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aqh.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kpi.hesvh.cn

Ruby: s.scan(/error/i)
来源：http://zuc.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bda.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://weo.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yez.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewo.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tvd.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://znr.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://huf.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lnk.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://akg.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nrs.xuanzx.com

================================================================================
来源：http://ayf.nanxinkj.top

J. 日期与时间
来源：http://ggg.mhx1999.top

================================================================================
来源：http://xzu.gzhubu.top

[J01] 获取当前时间
来源：http://esr.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hyd.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hut.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://zoa.svipenyu.cn

TS:   new Date();  Date.now()
来源：http://btq.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://try.hesvh.cn

Go:   time.Now()
来源：http://rlm.dianchejie.cn

Ruby: Time.now
来源：http://myn.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kqz.gogol.net.cn

[J02] 格式化输出
来源：http://ume.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://frc.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://usd.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wik.dashuyun.cn

TS:   d.toISOString()
来源：http://kus.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://czt.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ymh.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xat.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://teu.aibaodan.cn


<!-- 参考信息 -->