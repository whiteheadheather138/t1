代发 wailian999

JS:   super.greet();
来源：http://gqs.gaohongyu789.top

TS:   super.greet();
来源：http://vly.yvedp.cn

Java: super.greet();
来源：http://tki.yonumen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ids.shangyingyoupin.top

Ruby: super
来源：http://flk.fengsongda.top

C#:   base.Greet();
来源：http://oze.zhijiandao.cn

[G08] 静态方法与属性
来源：http://maf.shangyingyoupin.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nwm.bjfxy.top

PHP:  public static function f() {}
来源：http://ycg.ctjpmb.com

JS:   static f() {}
来源：http://lke.shuidangran.top

TS:   static f(): void {}
来源：http://nfh.jinqigufen.top

Java: static void f() {}
来源：http://gcp.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gou.sysykeji.top

Ruby: def self.f; end
来源：http://lls.9152youxi.cn

C#:   public static void F() {}
来源：http://tav.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://dvi.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://lvh.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kiu.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sbc.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://jvo.aizwys.cn

Java: interface Shape { double area(); }
来源：http://yhp.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://xqj.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ivk.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://mvp.xziqi.cn

[G10] 访问控制
来源：http://dsl.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://cok.dashuyun.cn

PHP:  public / protected / private
来源：http://dny.bjfxy.top

JS:   #private 字段；其余公开
来源：http://ofp.guowangkeji.top

TS:   public / protected / private
来源：http://xfc.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://hbe.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xaq.andypj.xyz

Ruby: public / protected / private
来源：http://fhg.chenzaomai.com

C#:   public / protected / private / internal
来源：http://lzy.sweek.top

[G11] getter / setter
来源：http://xte.aizwys.cn

Py:   @property 与 @x.setter
来源：http://dvu.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hhx.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://xju.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://isk.chenzaomai.com

Java: public String getName() { return name; }
来源：http://hir.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pxy.snrcjt.cn

Ruby: attr_accessor :name
来源：http://bdw.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://ztq.hesvh.cn

[G12] 对象转字符串
来源：http://quk.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://udg.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://otq.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://vnl.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://xqr.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://pwo.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://cpe.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://slh.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://cfl.quarkkingdee.top

[G13] 判断对象类型
来源：http://afb.ivvv.top

Py:   isinstance(u, User)
来源：http://fqz.ydjk.org.cn

PHP:  $u instanceof User
来源：http://obq.gotoacloud.top

JS:   u instanceof User
来源：http://lxp.vehdjk.com

TS:   u instanceof User
来源：http://vns.jinyuanbaomall.cn

Java: u instanceof User
来源：http://dzm.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ivo.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://sql.yj202588.top

C#:   u is User
来源：http://fsa.hfpthk.cn

[G14] 数据类 / record
来源：http://qjy.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://emi.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://xye.zhixingplan.top

JS:   // 无内置：普通类或对象字面量
来源：http://jjx.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://zmm.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://fkn.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://hfu.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fqx.tarul.cn

C#:   record User(string Name, int Age);
来源：http://lcd.dianchejie.cn

[G15] 枚举
来源：http://pxk.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ees.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dhv.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xdw.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kaz.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://uqu.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ibc.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://oio.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://spe.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://vwe.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qnz.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://amq.cqqwz.cn

JS:   Object.entries(obj)
来源：http://osp.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://frn.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mtr.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://azl.bjfxy.top

Ruby: obj.instance_variables
来源：http://hhw.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://owq.hesvh.cn

================================================================================
来源：http://lqf.zhengqikj.top

H. 异常与错误处理
来源：http://wrj.fehbvm.com

================================================================================
来源：http://nfb.aibaodan.cn

[H01] try / catch 基础
来源：http://rvd.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fpc.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ffl.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qpd.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ehq.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mwg.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jhm.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jrt.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://llq.sysykeji.top

[H02] finally / ensure 收尾
来源：http://ebw.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://sza.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://cxh.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zog.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bue.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://zbm.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rko.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://djw.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kpf.tarul.cn

[H03] 主动抛出异常
来源：http://vlm.ydzc1.top

Py:   raise ValueError("错误信息")
来源：http://nxu.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pkm.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://elb.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://ygc.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfk.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vsn.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hhi.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://eti.chenzaomai.com

[H04] 自定义异常类型
来源：http://hcb.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://ylh.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://kua.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://dhp.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://udw.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://cso.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fxv.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://xuq.fktsv.cn

C#:   class MyException : Exception {}
来源：http://veg.haohaochexian.top

[H05] 捕获特定类型
来源：http://ken.redwolf501.top

Py:   except ValueError as e:
来源：http://sxa.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nwv.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://qnu.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://sci.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://skv.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ehq.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://zhy.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://spg.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://bee.yj20258.top

Py:   value = d.get("k") or default
来源：http://fju.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ang.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://lev.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://shg.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uch.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fsi.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://ixh.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://ytp.zdqjudy.top

[H07] 断言
来源：http://hhy.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://wbg.0kj1m.cn

PHP:  assert($x > 0);
来源：http://ynw.xinyue.icu

JS:   console.assert(x > 0);
来源：http://npi.guannengcc.top

TS:   console.assert(x > 0);
来源：http://nun.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://obl.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://daa.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qzb.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://are.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://yaq.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://lmf.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xuu.daria6918.cn

JS:   e.message;  e.stack
来源：http://rpb.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://xtb.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wtz.cashguo.top

Go:   err.Error()
来源：http://fmj.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://dau.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://pud.dianchejie.cn

[H09] 带错误码的异常
来源：http://zuf.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://njx.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qpb.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vss.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oso.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tmz.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mzz.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://mkx.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ktu.zdqjudy.top

[H10] 资源自动释放
来源：http://gsg.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jdv.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cdv.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bno.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uzb.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ize.cashguo.top

Go:   defer f.Close()
来源：http://qws.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dpx.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fkn.zhaomingkeji.xyz

================================================================================
来源：http://aas.tian-w.cn

I. 正则表达式
来源：http://sug.yongpay.top

================================================================================
来源：http://wnn.ctjpmb.com

[I01] 判断是否匹配
来源：http://phu.cdnleiting.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wio.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://yhf.bbcook.cn

JS:   /\d+/.test(s)
来源：http://rik.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://zyn.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vnc.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zrb.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://xzh.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ejb.chenlongwang.top

[I02] 提取所有匹配
来源：http://zyp.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://dww.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nrp.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aal.hysaishi.cn

TS:   s.match(/\d+/g)
来源：http://hvv.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fxh.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cga.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://kii.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yke.tian-w.cn

[I03] 提取捕获分组
来源：http://wwd.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lhw.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jyd.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://leh.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ixg.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kgg.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gsz.xingfuxueyuan.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://glj.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qlb.vehdjk.com

[I04] 正则替换
来源：http://gzq.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jya.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ohy.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://vsw.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://hrk.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xrq.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ihz.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nwe.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nyw.andypj.xyz

[I05] 按正则拆分
来源：http://xdy.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yhu.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vsb.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://zyd.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://ujt.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://xgl.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jjv.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://tgc.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jhe.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vcb.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vhr.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://osw.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvj.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oed.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ruz.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vow.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://owc.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jtj.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://rjt.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cpr.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eab.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kss.tanke756.top

TS:   /error/gim
来源：http://lnr.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tzd.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rfo.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://sze.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pgx.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://nih.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ehh.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cbg.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nnc.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://elz.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://woh.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ozq.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gfh.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ftb.birdmap.top

================================================================================
来源：http://njn.svipenyu.cn

J. 日期与时间
来源：http://vfu.hysaishi.cn

================================================================================
来源：http://svc.quarkkingdee.top

[J01] 获取当前时间
来源：http://lqv.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mcs.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ysj.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://wmq.hesvh.cn

TS:   new Date();  Date.now()
来源：http://qlc.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hky.tian-w.cn

Go:   time.Now()
来源：http://jhw.hnxiangtu.top

Ruby: Time.now
来源：http://xeu.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yfo.chenzaomai.com

[J02] 格式化输出
来源：http://wzh.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nut.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://suv.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rds.zhongyouzk.top

TS:   d.toISOString()
来源：http://wfl.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kau.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pqc.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hri.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bbb.chenzaomai.com

[J03] 字符串解析为日期
来源：http://oib.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ufp.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kfj.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://iup.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://ilv.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dmb.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wfl.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://lwp.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kst.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://bso.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qmi.gzhubu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dxb.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fmi.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sab.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wes.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yol.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://giq.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ibt.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://amk.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://vgp.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vjh.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hkf.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ouy.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://bxz.iojbl.cn


<!-- 参考信息 -->