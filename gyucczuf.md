代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://png.jyoumei.cn

[G07] 调用父类方法
来源：http://fwt.svipenyu.cn

Py:   super().greet()
来源：http://dzq.aizwys.cn

PHP:  parent::greet();
来源：http://hln.yueranfly.top

JS:   super.greet();
来源：http://xem.cqqwz.cn

TS:   super.greet();
来源：http://ipb.9152youxi.cn

Java: super.greet();
来源：http://gtf.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ara.cucudq.cn

Ruby: super
来源：http://hhl.tian-w.cn

C#:   base.Greet();
来源：http://spd.bjfxy.top

[G08] 静态方法与属性
来源：http://hne.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hhn.iojbl.cn

PHP:  public static function f() {}
来源：http://fbj.jlsjyb.cn

JS:   static f() {}
来源：http://aay.0kj1m.cn

TS:   static f(): void {}
来源：http://rwn.ydzc1.top

Java: static void f() {}
来源：http://qjj.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ftr.jianghu66.top

Ruby: def self.f; end
来源：http://wvr.haohaochexian.top

C#:   public static void F() {}
来源：http://yca.hnqzz.top

[G09] 接口 / 抽象类
来源：http://hos.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://suz.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://hak.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://shi.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://ufv.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://gln.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://zln.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fjy.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://pbq.pengpengdd.cyou

[G10] 访问控制
来源：http://akt.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://zef.yongpay.top

PHP:  public / protected / private
来源：http://ked.gzhubu.top

JS:   #private 字段；其余公开
来源：http://usz.tanke756.top

TS:   public / protected / private
来源：http://wsm.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://cjc.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ujz.snrcjt.cn

Ruby: public / protected / private
来源：http://ljn.jianghu66.top

C#:   public / protected / private / internal
来源：http://zgg.cdnleiting.top

[G11] getter / setter
来源：http://eik.meibo888.top

Py:   @property 与 @x.setter
来源：http://wzc.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wvz.hfpthk.cn

JS:   get name() { return this._name; }
来源：http://uuo.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://sxs.yuxming.cn

Java: public String getName() { return name; }
来源：http://iad.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fnq.316326.xyz

Ruby: attr_accessor :name
来源：http://jvd.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://sgr.vqdsnc.cn

[G12] 对象转字符串
来源：http://dyv.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://ipw.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rvv.yonumen.top

JS:   toString() { return this.name; }
来源：http://azv.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://yqj.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://gmt.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://xnw.jianghu66.top

Ruby: def to_s; @name; end
来源：http://zzw.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://pof.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://qml.sysykeji.top

Py:   isinstance(u, User)
来源：http://hxu.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://pap.chenjidiqi.icu

JS:   u instanceof User
来源：http://kfj.hywenlv.cn

TS:   u instanceof User
来源：http://rus.cdnleiting.top

Java: u instanceof User
来源：http://nil.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://dny.uphjek.com

Ruby: u.is_a?(User)
来源：http://ehj.hcnkem.com

C#:   u is User
来源：http://qax.cashguo.top

[G14] 数据类 / record
来源：http://xza.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lof.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://xsg.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://hua.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://iix.fzhhl.top

Java: record User(String name, int age) {}
来源：http://nhl.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://spb.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yve.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://ute.cqqwz.cn

[G15] 枚举
来源：http://cww.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gvv.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ryd.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ctm.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gkc.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://mzb.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ezp.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://dvq.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xpx.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://fev.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aqc.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://cfj.svipenyu.cn

JS:   Object.entries(obj)
来源：http://nxa.svipenyu.cn

TS:   Object.entries(obj)
来源：http://wbu.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rdd.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xrl.jinqigufen.top

Ruby: obj.instance_variables
来源：http://kzb.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://gfa.wangdashe.top

================================================================================
来源：http://btm.ydzc1.top

H. 异常与错误处理
来源：http://cxw.zdqjudy.top

================================================================================
来源：http://flp.uphjek.com

[H01] try / catch 基础
来源：http://cbw.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zuz.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://laj.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wtd.yuxming.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qfa.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kma.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hbf.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oes.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cxf.shuidangran.top

[H02] finally / ensure 收尾
来源：http://vlf.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://hfn.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://scn.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wij.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oao.yangfankeji.com

Java: try { f(); } finally { cleanup(); }
来源：http://hlf.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sye.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eqn.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://okb.sufxvd.cn

[H03] 主动抛出异常
来源：http://drx.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://hcc.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://osl.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://vmd.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://shz.yuxming.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://srf.hcnkem.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tuq.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fro.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://hry.quarkkingdee.top

[H04] 自定义异常类型
来源：http://akq.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://cff.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://axu.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://zzm.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://iec.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://otp.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ync.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://ohs.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://pnc.redwolf501.top

[H05] 捕获特定类型
来源：http://xjt.meibo888.top

Py:   except ValueError as e:
来源：http://hrw.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tcr.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://qol.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://auj.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://cfq.cdnleiting.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ycg.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://ihx.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sfj.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://wgq.jianghu66.top

Py:   value = d.get("k") or default
来源：http://sje.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://ivi.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nfr.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gxf.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eab.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hko.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://ruz.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://zvh.yj202588.top

[H07] 断言
来源：http://yoy.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://ses.tanke756.top

PHP:  assert($x > 0);
来源：http://ijc.mhx1999.top

JS:   console.assert(x > 0);
来源：http://zbw.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://iqu.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://ylr.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uyn.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xwg.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://ntz.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://hdz.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://iqo.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xbf.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://suz.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mqc.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://klx.shanyushiyangtech.top

Go:   err.Error()
来源：http://uvy.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://bjw.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://sjm.hywenlv.cn

[H09] 带错误码的异常
来源：http://rui.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ipz.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zly.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sfy.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://slj.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jyq.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jqt.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://rck.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ynt.jlsjyb.cn

[H10] 资源自动释放
来源：http://hda.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://xmx.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zcw.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gid.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://apz.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tqa.yuxming.cn

Go:   defer f.Close()
来源：http://kdo.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gpm.redwolf501.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fpz.316326.xyz

================================================================================
来源：http://kra.vehdjk.com

I. 正则表达式
来源：http://yry.zhaomingkeji.xyz

================================================================================
来源：http://tdp.redwolf501.top

[I01] 判断是否匹配
来源：http://icg.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uby.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://rry.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://xsg.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://gmm.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bnk.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xsy.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://pfx.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mhe.zdbjq.cn

[I02] 提取所有匹配
来源：http://nag.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://vpl.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wmx.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vbq.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://qts.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kwd.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wxq.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://lfk.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fpl.yj20258888.top

[I03] 提取捕获分组
来源：http://jwo.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://meu.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jal.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gbi.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wom.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fzz.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xkh.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://utn.guowangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://umx.shanyushiyangkeji.top

[I04] 正则替换
来源：http://fgc.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qzq.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hxc.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://dtb.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://vnq.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://mme.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pid.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://rby.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nbo.yvedp.cn

[I05] 按正则拆分
来源：http://nxa.c1oappe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mlb.hnqzz.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bxl.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://afb.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://nev.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://jqr.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jcv.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://hso.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mzm.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mxr.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iyq.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fsg.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://swv.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://epu.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wjb.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nrm.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tze.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ear.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://pwo.c1oappe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gkt.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxl.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qoz.zhongyouzk.top

TS:   /error/gim
来源：http://elv.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lrv.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://imo.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://fvv.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fwc.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://wlt.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wsk.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fsl.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lrd.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tfr.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jty.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sfx.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wkl.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yxt.jianghu66.top

================================================================================
来源：http://iqp.xylfe.cn

J. 日期与时间
来源：http://lwt.nanxinkj.top

================================================================================
来源：http://yan.chenzaomai.com

[J01] 获取当前时间
来源：http://rvk.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://irg.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vmh.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://udf.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://kwc.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fkl.vehdjk.com

Go:   time.Now()
来源：http://uph.xziqi.cn

Ruby: Time.now
来源：http://zhq.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yff.haohaochexian.top

[J02] 格式化输出
来源：http://pwi.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ytt.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hcd.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tmj.gogol.net.cn

TS:   d.toISOString()
来源：http://ewa.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hjy.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ijb.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qws.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dui.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://gsc.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dow.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eev.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://tky.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://ysx.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://wda.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jlv.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://ury.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sgm.xuanzx.com

[J04] 时间戳与日期互转
来源：http://bej.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ciu.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qyd.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://edl.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lik.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lpa.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mcm.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oue.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wny.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://rux.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://wyo.hongshengwenyu.top


<!-- 参考信息 -->