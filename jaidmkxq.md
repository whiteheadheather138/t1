代发 wailian999

Java: class Admin extends User {}
来源：http://qbd.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bcl.redwolf501.top

Ruby: class Admin < User; end
来源：http://tid.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://yoa.zhaomingkeji.xyz

[G06] 重写方法
来源：http://ufj.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://mqs.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eiu.cashguo.top

JS:   greet() { return "admin"; }
来源：http://tjl.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://bql.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://geb.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dai.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://ras.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://qza.aibaodan.cn

[G07] 调用父类方法
来源：http://rmy.havefunace.top

Py:   super().greet()
来源：http://xmr.zhoulong.xyz

PHP:  parent::greet();
来源：http://bij.hysaishi.cn

JS:   super.greet();
来源：http://phq.ppjwa.cn

TS:   super.greet();
来源：http://zky.andypj.xyz

Java: super.greet();
来源：http://sjn.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xxd.uphjek.com

Ruby: super
来源：http://nxl.yueranfly.top

C#:   base.Greet();
来源：http://pvf.fzhhl.top

[G08] 静态方法与属性
来源：http://gaz.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://crp.sxryk.cn

PHP:  public static function f() {}
来源：http://mqd.tian-w.cn

JS:   static f() {}
来源：http://wss.ydzc1.top

TS:   static f(): void {}
来源：http://prz.hywenlv.cn

Java: static void f() {}
来源：http://pkh.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://grv.gotoacloud.top

Ruby: def self.f; end
来源：http://zaf.yongpay.top

C#:   public static void F() {}
来源：http://nry.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://wcu.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://dnd.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://cfc.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mya.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://lzb.52xcode.cn

Java: interface Shape { double area(); }
来源：http://idz.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://fmc.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oih.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://ywl.meibo888.top

[G10] 访问控制
来源：http://ytz.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://bjp.tian-w.cn

PHP:  public / protected / private
来源：http://oft.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://tbo.hcnkem.com

TS:   public / protected / private
来源：http://mbe.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://tsp.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qgb.hnxiangtu.top

Ruby: public / protected / private
来源：http://ewp.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://enw.hysaishi.cn

[G11] getter / setter
来源：http://uho.yvedp.cn

Py:   @property 与 @x.setter
来源：http://cul.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jfi.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://ugn.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://ujq.hcnkem.com

Java: public String getName() { return name; }
来源：http://ajj.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gde.zhengqikj.top

Ruby: attr_accessor :name
来源：http://zrx.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://koa.yuanzhike.top

[G12] 对象转字符串
来源：http://ymh.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://ohn.zhijiandao.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cem.iojbl.cn

JS:   toString() { return this.name; }
来源：http://cxy.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://zyx.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://xzk.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tfy.havefunace.top

Ruby: def to_s; @name; end
来源：http://mjt.yonumen.top

C#:   public override string ToString() => Name;
来源：http://pum.fengsongda.top

[G13] 判断对象类型
来源：http://boj.zhengqikj.top

Py:   isinstance(u, User)
来源：http://pxh.zhijiandao.cn

PHP:  $u instanceof User
来源：http://nyw.xylfe.cn

JS:   u instanceof User
来源：http://btq.wangshuangyany.cn

TS:   u instanceof User
来源：http://pzc.zhiwuduotai.top

Java: u instanceof User
来源：http://szi.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kqk.wangdashe.top

Ruby: u.is_a?(User)
来源：http://sku.cdnleiting.top

C#:   u is User
来源：http://iza.fengsongda.top

[G14] 数据类 / record
来源：http://oxl.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oul.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://cjk.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://arw.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://nip.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://wsw.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://gzj.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ttd.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://lgc.aizwys.cn

[G15] 枚举
来源：http://odd.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gwp.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://sqr.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fey.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kte.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://mnq.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uvh.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://mwu.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mlp.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://rqt.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zaz.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://cqp.jiagoushi.top

JS:   Object.entries(obj)
来源：http://wff.nanxinkj.top

TS:   Object.entries(obj)
来源：http://zfo.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cnz.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://uzs.yuxming.cn

Ruby: obj.instance_variables
来源：http://pvz.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://gsj.tian-w.cn

================================================================================
来源：http://rbd.dianchejie.cn

H. 异常与错误处理
来源：http://rqu.shangyingyoupin.top

================================================================================
来源：http://wuo.zhixingplan.top

[H01] try / catch 基础
来源：http://lrg.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bbl.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tbw.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oby.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://chu.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zna.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fnw.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fwj.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pjz.nwbrower.top

[H02] finally / ensure 收尾
来源：http://yhx.zycfv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uhy.9152youxi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hxs.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://gho.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cre.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://xhz.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ozd.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hgh.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yng.havefunace.top

[H03] 主动抛出异常
来源：http://rqk.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://jei.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ojm.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://sgv.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://kjj.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vzb.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kyk.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cmn.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://fgt.mhx1999.top

[H04] 自定义异常类型
来源：http://uew.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://zme.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://sab.zhiwuduotai.top

JS:   class MyError extends Error {}
来源：http://anf.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://loh.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://lbz.52xcode.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ttf.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://bch.fzhhl.top

C#:   class MyException : Exception {}
来源：http://zqg.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://sru.52xcode.cn

Py:   except ValueError as e:
来源：http://zao.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tbm.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://ifn.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://dmq.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://igo.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ogq.sweek.top

Ruby: rescue ArgumentError => e
来源：http://ihu.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sjq.fktsv.cn

[H06] 可选值 / 空值安全访问
来源：http://hrk.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://nuc.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kiz.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://ffj.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iik.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wrz.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://noz.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://uwb.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://qze.daria6918.cn

[H07] 断言
来源：http://kdt.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://ldn.gotoacloud.top

PHP:  assert($x > 0);
来源：http://coz.mhx1999.top

JS:   console.assert(x > 0);
来源：http://ebg.daxiang520.top

TS:   console.assert(x > 0);
来源：http://kdf.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://caf.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://icc.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hsf.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://nvx.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://dkn.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://zmi.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mmq.meibo888.top

JS:   e.message;  e.stack
来源：http://mlw.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kwg.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://msb.bjfxy.top

Go:   err.Error()
来源：http://xgu.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://hco.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://gjr.chenlongwang.top

[H09] 带错误码的异常
来源：http://avh.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mqm.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jlx.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aqo.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bto.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dyt.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lvv.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://xkb.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://psu.guannengcc.top

[H10] 资源自动释放
来源：http://swd.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kvl.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://akw.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pib.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lwd.xingfuxueyuan.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eur.yanxiufei.cn

Go:   defer f.Close()
来源：http://wag.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://frj.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ifq.fzhhl.top

================================================================================
来源：http://mjz.feifeiyinyue.top

I. 正则表达式
来源：http://wgs.smart0.xyz

================================================================================
来源：http://xzz.ybcxt.top

[I01] 判断是否匹配
来源：http://ahg.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oia.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oaw.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://tkg.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://kec.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gsc.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vsm.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://atx.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vog.zhijiandao.cn

[I02] 提取所有匹配
来源：http://iah.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://ynl.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jsf.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jxi.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://ppb.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zja.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xzz.xingfuxueyuan.xyz

Ruby: s.scan(/\d+/)
来源：http://trm.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://loj.cdnleiting.top

[I03] 提取捕获分组
来源：http://jlc.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ifw.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qca.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cri.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nfj.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://agq.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nna.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iaz.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://elu.vqdsnc.cn

[I04] 正则替换
来源：http://fly.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kdt.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://una.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://xnc.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://xfv.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://bcj.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ees.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xzd.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yli.xinyue.icu

[I05] 按正则拆分
来源：http://upe.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://mzg.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mez.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://fom.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://der.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://pot.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zpg.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://xpn.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tor.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cki.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tin.andypj.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jcn.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cii.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kze.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yxm.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vkl.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kzs.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dmq.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://aex.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bnw.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fvx.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ytl.guannengcc.top

TS:   /error/gim
来源：http://bza.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kyn.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://buh.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://chu.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fpb.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://sjy.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gpx.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jwv.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwl.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xju.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://srs.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gae.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lpf.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fvt.dianchejie.cn

================================================================================
来源：http://fso.sxryk.cn

J. 日期与时间
来源：http://akn.gogol.net.cn

================================================================================
来源：http://lry.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://tpn.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://jxx.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pux.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://hdc.birdmap.top

TS:   new Date();  Date.now()
来源：http://htv.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hmd.fehbvm.com

Go:   time.Now()
来源：http://xzr.jinqigufen.top

Ruby: Time.now
来源：http://xad.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vzu.c1oappe.top

[J02] 格式化输出
来源：http://vnx.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qyf.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jzd.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mnj.zdbjq.cn

TS:   d.toISOString()
来源：http://chz.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tqf.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://avo.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nwz.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jxc.dashuyun.cn

[J03] 字符串解析为日期
来源：http://qla.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://egl.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gnt.yongpay.top

JS:   new Date("2024-01-02")
来源：http://bmz.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://hup.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://its.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vuk.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://yfn.xuanzx.com


<!-- 参考信息 -->