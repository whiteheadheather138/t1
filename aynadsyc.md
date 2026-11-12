代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://mlt.cucudq.cn

[G07] 调用父类方法
来源：http://xqd.chenjidiqi.icu

Py:   super().greet()
来源：http://qwd.meibo888.top

PHP:  parent::greet();
来源：http://eim.zhiwuduotai.top

JS:   super.greet();
来源：http://oyg.bbcook.cn

TS:   super.greet();
来源：http://uda.jlsjyb.cn

Java: super.greet();
来源：http://zny.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bva.dashuyun.cn

Ruby: super
来源：http://ofw.yfazqb.com

C#:   base.Greet();
来源：http://qza.bjfxy.top

[G08] 静态方法与属性
来源：http://lsy.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bjg.shuidangran.top

PHP:  public static function f() {}
来源：http://tfd.havefunace.top

JS:   static f() {}
来源：http://hns.zycfv.cn

TS:   static f(): void {}
来源：http://tzw.birdmap.top

Java: static void f() {}
来源：http://idi.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mjd.gotoacloud.top

Ruby: def self.f; end
来源：http://man.ehwqpu.com

C#:   public static void F() {}
来源：http://vhv.tian-w.cn

[G09] 接口 / 抽象类
来源：http://buf.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ocx.havefunace.top

PHP:  interface Shape { public function area(): float; }
来源：http://krh.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://eem.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://oqg.yvedp.cn

Java: interface Shape { double area(); }
来源：http://lde.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://nkk.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jgk.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://nhl.chenjidiqi.icu

[G10] 访问控制
来源：http://fah.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://bzo.pengpengdd.cyou

PHP:  public / protected / private
来源：http://knk.epnwcf.com

JS:   #private 字段；其余公开
来源：http://apb.hongshengwenyu.top

TS:   public / protected / private
来源：http://mfj.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://sdq.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fzm.daxiang520.top

Ruby: public / protected / private
来源：http://lti.yuxming.cn

C#:   public / protected / private / internal
来源：http://btg.uphjek.com

[G11] getter / setter
来源：http://aoc.wangdashe.top

Py:   @property 与 @x.setter
来源：http://jpl.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jsu.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://wzb.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://tfb.0kj1m.cn

Java: public String getName() { return name; }
来源：http://rvk.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kgp.hcnkem.com

Ruby: attr_accessor :name
来源：http://kbv.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://iah.hnxiangtu.top

[G12] 对象转字符串
来源：http://vmc.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://tha.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://elb.yj202588.top

JS:   toString() { return this.name; }
来源：http://uyw.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://vkv.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://eir.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://vbt.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://zeb.yongpay.top

C#:   public override string ToString() => Name;
来源：http://ghw.chenlongwang.top

[G13] 判断对象类型
来源：http://ilt.yfazqb.com

Py:   isinstance(u, User)
来源：http://kvr.zhixingplan.top

PHP:  $u instanceof User
来源：http://vhj.yongpay.top

JS:   u instanceof User
来源：http://giv.shangyingyoupin.top

TS:   u instanceof User
来源：http://ufk.ydjk.org.cn

Java: u instanceof User
来源：http://bmn.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://omq.jinqigfzy.top

Ruby: u.is_a?(User)
来源：http://sqg.dashuyun.cn

C#:   u is User
来源：http://ffs.fktsv.cn

[G14] 数据类 / record
来源：http://qof.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vkf.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://qeq.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://xlp.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://ips.wangdashe.top

Java: record User(String name, int age) {}
来源：http://jkm.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://gpv.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qyy.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://vbg.jianghu66.top

[G15] 枚举
来源：http://znf.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://roe.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ojm.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zim.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wlh.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://sts.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gzi.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://nyv.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ovw.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://qon.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qpi.meibo888.top

PHP:  get_object_vars($obj);
来源：http://vwx.zhengqikj.top

JS:   Object.entries(obj)
来源：http://lzf.redwolf501.top

TS:   Object.entries(obj)
来源：http://dwp.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iif.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://mgr.gzhubu.top

Ruby: obj.instance_variables
来源：http://xlf.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://oqb.cucudq.cn

================================================================================
来源：http://sno.jiagoushi.top

H. 异常与错误处理
来源：http://rbi.pycfn.com

================================================================================
来源：http://oco.chenjidiqi.icu

[H01] try / catch 基础
来源：http://tbv.hywenlv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jgl.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lqq.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nel.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxx.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://anv.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kcf.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsj.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ilq.iojbl.cn

[H02] finally / ensure 收尾
来源：http://gsk.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ztg.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vqi.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ccp.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://typ.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://ivn.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://llh.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ybj.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://naq.gaohongyu789.top

[H03] 主动抛出异常
来源：http://xhb.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://uxk.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mxe.pycfn.com

JS:   throw new Error("错误信息");
来源：http://bst.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://tti.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://auv.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gwa.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qic.cdnleiting.top

C#:   throw new ArgumentException("错误信息");
来源：http://jbd.vqdsnc.cn

[H04] 自定义异常类型
来源：http://zle.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://hal.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://rnu.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://ijj.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://zva.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://rfr.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oto.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://nrv.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://bbr.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://rzd.yanxiufei.cn

Py:   except ValueError as e:
来源：http://uel.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://woj.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://pag.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://ebf.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://yjy.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://axk.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://jsg.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eag.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://yxg.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://phz.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://lsj.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://olv.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://tes.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://joz.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://obv.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://izr.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://rte.hcnkem.com

[H07] 断言
来源：http://pok.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://opz.fktsv.cn

PHP:  assert($x > 0);
来源：http://ewd.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://onz.xziqi.cn

TS:   console.assert(x > 0);
来源：http://rvm.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://uiu.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgp.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sxk.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://lzs.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://ciw.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://hwc.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hre.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://pyv.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jem.zhengqikj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fon.snrcjt.cn

Go:   err.Error()
来源：http://xiq.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://oap.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://hqc.jlsjyb.cn

[H09] 带错误码的异常
来源：http://nsb.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vxv.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://odc.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kls.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jvw.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jhl.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://onb.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://lhn.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://phi.zhijiandao.cn

[H10] 资源自动释放
来源：http://mli.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pxz.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mmk.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hzo.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xal.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://brm.nanxuanxn.top

Go:   defer f.Close()
来源：http://iwh.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nqw.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eqy.hesvh.cn

================================================================================
来源：http://sjp.52xcode.cn

I. 正则表达式
来源：http://klq.yongpay.top

================================================================================
来源：http://wrk.xylfe.cn

[I01] 判断是否匹配
来源：http://ttc.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bjy.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://pey.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://wrr.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://tuw.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vsx.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sqf.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://vuy.zdbjq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://joh.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://yds.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://xqo.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://alq.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oba.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://zrm.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uhb.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rpr.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://dqm.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tvx.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://jiq.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mbj.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://krv.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hqo.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jce.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lmo.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eoi.tarul.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cfl.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zkn.jinqigufen.top

[I04] 正则替换
来源：http://kiq.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://izz.bbcook.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eyp.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://bbh.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://suu.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nmq.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nvr.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pfk.fengsongda.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rln.zhiwuduotai.top

[I05] 按正则拆分
来源：http://mew.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zpq.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oib.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://wvh.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://vyh.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://puc.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://onw.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ijr.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jeg.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://paz.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kee.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dpd.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhs.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mih.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gmt.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://deo.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ygw.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ius.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://vpb.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kgg.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ygn.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nfy.zhijiandao.cn

TS:   /error/gim
来源：http://vmd.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gru.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qov.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://fxm.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fqv.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://ynu.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vmc.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nrz.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zbf.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nmr.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ndi.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pfz.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://teg.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tui.yj20258888.top

================================================================================
来源：http://fnj.hongshengwenyu.top

J. 日期与时间
来源：http://qxv.sysykeji.top

================================================================================
来源：http://bsp.hammf.cn

[J01] 获取当前时间
来源：http://mhe.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://guw.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://anv.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://ori.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://xjj.tarul.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ixi.0kj1m.cn

Go:   time.Now()
来源：http://eck.wangshuangyany.cn

Ruby: Time.now
来源：http://pcl.mhx1999.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lnb.hongshengwenyu.top

[J02] 格式化输出
来源：http://wxa.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wek.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vmo.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pyb.yj20258.top

TS:   d.toISOString()
来源：http://ekq.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rwb.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hki.hnxiangtu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://beb.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://joq.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://wxg.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eyg.jyoumei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sdy.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://jxr.cdnleiting.top

TS:   new Date("2024-01-02")
来源：http://gqf.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://emm.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nfb.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://omn.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mww.mhx1999.top

[J04] 时间戳与日期互转
来源：http://ijo.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nto.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hmu.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://doz.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rdw.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uwt.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tdh.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vop.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wph.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://lqs.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://tva.gaohongyu789.top


<!-- 参考信息 -->