代发 wailian999

Ruby: super
来源：http://czs.ydjk.org.cn

C#:   base.Greet();
来源：http://asp.cqqwz.cn

[G08] 静态方法与属性
来源：http://uyq.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fuc.yj20258.top

PHP:  public static function f() {}
来源：http://lwj.xziqi.cn

JS:   static f() {}
来源：http://xya.ctjpmb.com

TS:   static f(): void {}
来源：http://fit.birdmap.top

Java: static void f() {}
来源：http://qof.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tco.shuidangran.top

Ruby: def self.f; end
来源：http://irq.havefunace.top

C#:   public static void F() {}
来源：http://whm.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://llf.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://qfl.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xuq.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lzy.ywan-chungtsiang.top

TS:   interface Shape { area(): number; }
来源：http://uul.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://dts.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://wfp.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qig.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://ktw.gogol.net.cn

[G10] 访问控制
来源：http://ayi.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://ask.zycfv.cn

PHP:  public / protected / private
来源：http://woz.sxryk.cn

JS:   #private 字段；其余公开
来源：http://lbf.ywan-chungtsiang.top

TS:   public / protected / private
来源：http://jka.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://ini.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dfb.yonumen.top

Ruby: public / protected / private
来源：http://jqj.c1oappe.top

C#:   public / protected / private / internal
来源：http://llw.feifeiyinyue.top

[G11] getter / setter
来源：http://ogd.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://xjn.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ppo.hammf.cn

JS:   get name() { return this._name; }
来源：http://ckc.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://kbk.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://cmb.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kic.yangfankeji.com

Ruby: attr_accessor :name
来源：http://lsn.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://vcu.zdqjudy.top

[G12] 对象转字符串
来源：http://odn.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://mpz.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://daz.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://bov.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://iro.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://tam.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://ieb.zycfv.cn

Ruby: def to_s; @name; end
来源：http://izd.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://ekp.hnxiangtu.top

[G13] 判断对象类型
来源：http://zvq.tarul.cn

Py:   isinstance(u, User)
来源：http://ozn.zhijiandao.cn

PHP:  $u instanceof User
来源：http://lxx.yvedp.cn

JS:   u instanceof User
来源：http://vmv.hesvh.cn

TS:   u instanceof User
来源：http://rty.fktsv.cn

Java: u instanceof User
来源：http://kxn.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pau.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://rix.ybcxt.top

C#:   u is User
来源：http://izk.cucudq.cn

[G14] 数据类 / record
来源：http://bhm.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cnd.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://twi.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://sjy.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://acp.cucudq.cn

Java: record User(String name, int age) {}
来源：http://bun.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://nvg.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ihq.kuanghao11.cn

C#:   record User(string Name, int Age);
来源：http://lgm.birdmap.top

[G15] 枚举
来源：http://iwv.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hjs.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wcc.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ybq.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uit.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://rhi.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kdz.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://lip.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ulz.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://vnt.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qkh.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://pvy.daxiang520.top

JS:   Object.entries(obj)
来源：http://oub.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://epw.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qpd.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ocq.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://rzp.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://vxw.gzhubu.top

================================================================================
来源：http://var.tanke756.top

H. 异常与错误处理
来源：http://edm.uphjek.com

================================================================================
来源：http://ljj.andypj.xyz

[H01] try / catch 基础
来源：http://esp.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qwe.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gyh.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gvj.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nas.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sap.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zcz.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bay.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iak.yj20258.top

[H02] finally / ensure 收尾
来源：http://hzi.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://opk.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://khz.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ecm.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lpd.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://ibp.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mva.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://unq.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fex.yuxming.cn

[H03] 主动抛出异常
来源：http://rpr.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://pfq.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jgw.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://hut.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://swj.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://iyq.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yam.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://her.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vfu.jinqigufen.top

[H04] 自定义异常类型
来源：http://ldr.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://urm.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kmw.zhaomingkeji.xyz

JS:   class MyError extends Error {}
来源：http://dvn.aizwys.cn

TS:   class MyError extends Error {}
来源：http://zmq.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://ptt.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qau.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://kyg.fzhhl.top

C#:   class MyException : Exception {}
来源：http://shl.guowangkeji.top

[H05] 捕获特定类型
来源：http://wdl.guowangkeji.top

Py:   except ValueError as e:
来源：http://qmn.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://saz.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://fdt.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://lco.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://daw.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hmy.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://tuu.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xxy.chenlongwang.top

[H06] 可选值 / 空值安全访问
来源：http://jrx.bjfxy.top

Py:   value = d.get("k") or default
来源：http://ehf.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://hye.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://enz.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://iey.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wam.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yee.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://rut.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://bgj.chenjidiqi.icu

[H07] 断言
来源：http://fgb.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://uva.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://qpd.yuxming.cn

JS:   console.assert(x > 0);
来源：http://hzj.jianghu66.top

TS:   console.assert(x > 0);
来源：http://tfo.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://dfm.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rio.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://qax.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://nyc.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://smk.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://xnz.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://upp.zhengqikj.top

JS:   e.message;  e.stack
来源：http://bsr.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zal.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dty.ivvv.top

Go:   err.Error()
来源：http://omd.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://wsm.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://mgy.vqdsnc.cn

[H09] 带错误码的异常
来源：http://isk.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eyb.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rsk.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qmt.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vet.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vyz.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://erh.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://rcn.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jyt.svipenyu.cn

[H10] 资源自动释放
来源：http://jue.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nvk.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dut.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mmm.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wox.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fxa.jyoumei.cn

Go:   defer f.Close()
来源：http://yds.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cse.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ywj.guannengcc.top

================================================================================
来源：http://rtx.yongpay.top

I. 正则表达式
来源：http://qkq.tianlin.xyz

================================================================================
来源：http://yms.havefunace.top

[I01] 判断是否匹配
来源：http://ypb.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sjl.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qez.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://ows.bbcook.cn

TS:   /\d+/.test(s)
来源：http://zlh.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ish.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tvq.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://lqe.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://chg.pycfn.com

[I02] 提取所有匹配
来源：http://nte.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://tpk.meibo888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nrl.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zdl.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://fqb.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://axm.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jxa.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://xag.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yxe.shuidangran.top

[I03] 提取捕获分组
来源：http://tyu.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tel.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bfi.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ovy.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://exx.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bld.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qap.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qsx.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nhc.hcnkem.com

[I04] 正则替换
来源：http://oro.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qkh.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cds.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uzc.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hnh.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://ryj.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qzx.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://jlo.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qku.9152youxi.cn

[I05] 按正则拆分
来源：http://nmf.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cdb.zhijiandao.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gzx.guowangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://oqz.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://ezv.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://jvf.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zru.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://dwt.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lnh.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bes.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bpe.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rcc.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tux.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://smw.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cjj.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hky.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zqq.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tcs.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://bzk.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://riu.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://khg.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cxa.wangshuangyany.cn

TS:   /error/gim
来源：http://xzy.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ffb.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wcj.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://yhm.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fhc.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://jdb.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bqr.jyoumei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://geo.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwx.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jsc.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dlq.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sxf.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ffr.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uit.yvedp.cn

================================================================================
来源：http://kww.xuetiantiany.cn

J. 日期与时间
来源：http://lml.quarkkingdee.top

================================================================================
来源：http://kvv.shanyushiyangkeji.top

[J01] 获取当前时间
来源：http://mgf.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fna.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rqd.bjfxy.top

JS:   new Date();  Date.now()
来源：http://jgx.c1oappe.top

TS:   new Date();  Date.now()
来源：http://qsn.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://log.fzhhl.top

Go:   time.Now()
来源：http://dxf.tarul.cn

Ruby: Time.now
来源：http://nol.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gke.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://dzj.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ioy.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hpi.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qne.fengsongda.top

TS:   d.toISOString()
来源：http://pwq.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jsp.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rvr.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ohk.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ala.yuanzhike.top

[J03] 字符串解析为日期
来源：http://jae.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vff.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://who.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://cid.yongpay.top

TS:   new Date("2024-01-02")
来源：http://wcg.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://hue.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ont.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://efj.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sqi.hammf.cn

[J04] 时间戳与日期互转
来源：http://zsw.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mwi.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zms.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cny.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tfb.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zyj.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ldq.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rwa.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xmr.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://qzr.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://crl.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xmb.yfazqb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mxa.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oud.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://yjb.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://njl.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://izc.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://qrm.yj20258.top

[J06] 计算两时间之差
来源：http://ham.fanxiaobao.xyz


<!-- 参考信息 -->