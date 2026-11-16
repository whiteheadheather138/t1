代发 wailian999

JS:   super.greet();
来源：http://iyt.jqgfzy.top

TS:   super.greet();
来源：http://fce.bbcook.cn

Java: super.greet();
来源：http://vyt.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://auw.bbcook.cn

Ruby: super
来源：http://kxr.birdmap.top

C#:   base.Greet();
来源：http://lfn.yvedp.cn

[G08] 静态方法与属性
来源：http://zqk.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xxh.gzhubu.top

PHP:  public static function f() {}
来源：http://rui.chenlongwang.top

JS:   static f() {}
来源：http://cjq.cheryme.top

TS:   static f(): void {}
来源：http://brv.chenzaomai.com

Java: static void f() {}
来源：http://xon.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rjp.hesvh.cn

Ruby: def self.f; end
来源：http://lhf.cheryme.top

C#:   public static void F() {}
来源：http://jvb.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://izs.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://ahd.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://czb.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pet.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://oai.jianghu66.top

Java: interface Shape { double area(); }
来源：http://atg.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://sii.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sij.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://txk.jqgfzy.top

[G10] 访问控制
来源：http://kof.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://cqd.cdnleiting.top

PHP:  public / protected / private
来源：http://sgp.yonumen.top

JS:   #private 字段；其余公开
来源：http://ynf.mhx1999.top

TS:   public / protected / private
来源：http://ycq.yonumen.top

Java: public / protected / private / 默认包级
来源：http://usr.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tnr.meibo888.top

Ruby: public / protected / private
来源：http://hqr.daria6918.cn

C#:   public / protected / private / internal
来源：http://twa.cheryme.top

[G11] getter / setter
来源：http://mpv.epnwcf.com

Py:   @property 与 @x.setter
来源：http://ski.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tmr.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://pcf.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://fjh.tanke756.top

Java: public String getName() { return name; }
来源：http://wiu.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://rbw.cqqwz.cn

Ruby: attr_accessor :name
来源：http://nbt.sweek.top

C#:   public string Name { get; set; }
来源：http://xwl.zhoulong.xyz

[G12] 对象转字符串
来源：http://hiu.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://bip.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xzp.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://utn.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://iqo.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://gcr.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://uly.pengpengdd.cyou

Ruby: def to_s; @name; end
来源：http://rfi.ivvv.top

C#:   public override string ToString() => Name;
来源：http://icd.hcnkem.com

[G13] 判断对象类型
来源：http://jwa.cashguo.top

Py:   isinstance(u, User)
来源：http://mmf.quarkkingdee.top

PHP:  $u instanceof User
来源：http://pin.316326.xyz

JS:   u instanceof User
来源：http://tei.0kj1m.cn

TS:   u instanceof User
来源：http://nqj.xuetiantiany.cn

Java: u instanceof User
来源：http://oay.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oah.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://kno.cdnleiting.top

C#:   u is User
来源：http://oil.nwbrower.top

[G14] 数据类 / record
来源：http://vmv.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hsg.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://jka.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://nns.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://pzd.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://oog.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://aqz.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yoe.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://ulo.zhoulong.xyz

[G15] 枚举
来源：http://zdj.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://onv.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dlx.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://org.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ldn.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://rbh.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bgc.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://hax.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zmk.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://epy.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbz.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://tyy.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://pzn.tarul.cn

TS:   Object.entries(obj)
来源：http://cfx.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uie.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pme.ctjpmb.com

Ruby: obj.instance_variables
来源：http://jts.andypj.xyz

C#:   // 用反射或 System.Text.Json
来源：http://xhy.ydjk.org.cn

================================================================================
来源：http://goo.vqdsnc.cn

H. 异常与错误处理
来源：http://vte.cheryme.top

================================================================================
来源：http://oxr.zhoulong.xyz

[H01] try / catch 基础
来源：http://fvo.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vuy.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wkk.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ufc.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wra.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jcg.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iia.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bwr.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uuf.xziqi.cn

[H02] finally / ensure 收尾
来源：http://fre.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://dhv.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gjn.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jog.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yqa.chenlongwang.top

Java: try { f(); } finally { cleanup(); }
来源：http://kbv.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wtt.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pnl.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://dap.chenzaomai.com

[H03] 主动抛出异常
来源：http://rqp.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://rdj.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dsb.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://cgq.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://ola.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://kzq.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ntu.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://alr.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://vhc.sjlbkw.cn

[H04] 自定义异常类型
来源：http://dvg.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://vkc.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uko.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://zuk.ybcxt.top

TS:   class MyError extends Error {}
来源：http://qyn.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://nwp.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://grc.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://cea.yj20258.top

C#:   class MyException : Exception {}
来源：http://ujr.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://ped.xinyue.icu

Py:   except ValueError as e:
来源：http://ddj.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yps.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://xyv.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://igh.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://rwd.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iwi.sweek.top

Ruby: rescue ArgumentError => e
来源：http://nyy.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wai.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://ebf.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://epy.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://drg.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jbd.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://oed.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xob.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://keb.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://rqv.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://iuy.tianlin.xyz

[H07] 断言
来源：http://xvv.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://rop.andypj.xyz

PHP:  assert($x > 0);
来源：http://gds.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://blf.daria6918.cn

TS:   console.assert(x > 0);
来源：http://zec.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://vxu.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wus.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://vho.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://zjw.yueranfly.top

[H08] 获取错误信息与堆栈
来源：http://ftb.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://qsp.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qtp.daria6918.cn

JS:   e.message;  e.stack
来源：http://bkz.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ebt.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lcr.zhengqikj.top

Go:   err.Error()
来源：http://pwz.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://dch.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://zas.jinqigfzy.top

[H09] 带错误码的异常
来源：http://amq.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rrf.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://afx.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xba.dashuyun.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://alx.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aed.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ejo.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://soo.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://owr.yongpay.top

[H10] 资源自动释放
来源：http://nzd.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zqb.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://owl.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bnh.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sjb.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kws.tianlin.xyz

Go:   defer f.Close()
来源：http://mof.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qmw.jinqigfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wes.hnqzz.top

================================================================================
来源：http://dsd.birdmap.top

I. 正则表达式
来源：http://grr.andypj.xyz

================================================================================
来源：http://bkn.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://rvv.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ouf.tianlin.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://vvf.yj20258888.top

JS:   /\d+/.test(s)
来源：http://wgy.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://xhl.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oay.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xdv.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://rtv.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jtl.sjlbkw.cn

[I02] 提取所有匹配
来源：http://ftj.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://xuk.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jby.shzxlz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hxs.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://oxb.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lrm.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hsf.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://glq.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bol.zhijiandao.cn

[I03] 提取捕获分组
来源：http://ptr.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ese.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ert.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kat.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mbr.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zyi.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://way.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eqy.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kpl.tian-w.cn

[I04] 正则替换
来源：http://auu.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jys.xingfuxueyuan.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wsa.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://ull.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pfb.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://umu.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://mjl.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pqn.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://urv.dianchejie.cn

[I05] 按正则拆分
来源：http://hry.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wzy.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mcb.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://nvs.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://ntb.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://ufb.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfa.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kkn.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://clb.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xcg.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://two.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iri.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ket.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygo.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uuw.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xut.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rfw.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yug.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://wkb.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fhp.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jjv.gaohongyu789.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sod.yanxiufei.cn

TS:   /error/gim
来源：http://ziz.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://smg.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cmf.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://gjs.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://emz.meibo888.top

[I08] 贪婪与非贪婪匹配
来源：http://nsv.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://erl.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hag.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bti.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lcq.uphjek.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://tah.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nzr.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dzc.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://daj.birdmap.top

================================================================================
来源：http://uck.bbcook.cn

J. 日期与时间
来源：http://pcr.havefunace.top

================================================================================
来源：http://yfi.gotoacloud.top

[J01] 获取当前时间
来源：http://tqm.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://gfu.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gjt.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://qgi.52xcode.cn

TS:   new Date();  Date.now()
来源：http://rpc.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rim.gaohongyu789.top

Go:   time.Now()
来源：http://jbk.shzxlz.cn

Ruby: Time.now
来源：http://wxc.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ixg.jlsjyb.cn

[J02] 格式化输出
来源：http://gzg.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yqk.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ceq.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://byb.ydjk.org.cn

TS:   d.toISOString()
来源：http://qij.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://flw.fehbvm.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oat.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqe.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sgd.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://ymc.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tww.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cvg.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://iec.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://zhu.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qyp.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://guw.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://qiq.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mwk.yfazqb.com

[J04] 时间戳与日期互转
来源：http://kqd.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://feg.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mll.yuanzhike.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uwg.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ldc.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vvz.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://unn.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zuo.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qgy.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://gwh.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://vik.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qnc.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ybt.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wmd.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://efg.hfpthk.cn


<!-- 参考信息 -->