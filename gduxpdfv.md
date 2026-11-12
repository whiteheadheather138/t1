代发 wailian999

JS:   super.greet();
来源：http://zoh.ivvv.top

TS:   super.greet();
来源：http://txy.fengsongda.top

Java: super.greet();
来源：http://pow.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bod.0kj1m.cn

Ruby: super
来源：http://txl.jinghuilouyu.cn

C#:   base.Greet();
来源：http://tkf.sjlbkw.cn

[G08] 静态方法与属性
来源：http://lgg.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yfg.zhongyouzk.top

PHP:  public static function f() {}
来源：http://ojw.sufxvd.cn

JS:   static f() {}
来源：http://wlv.yj20258.top

TS:   static f(): void {}
来源：http://fzu.jinqigufen.top

Java: static void f() {}
来源：http://cjc.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jxc.ydjk.org.cn

Ruby: def self.f; end
来源：http://pxf.meibo888.top

C#:   public static void F() {}
来源：http://qtf.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://tck.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://lgu.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://dhb.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xlh.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://zmg.yvedp.cn

Java: interface Shape { double area(); }
来源：http://srw.aibaodan.cn

Go:   type Shape interface { Area() float64 }
来源：http://kqa.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://azs.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://osw.birdmap.top

[G10] 访问控制
来源：http://zwt.jqgfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://chl.gotoacloud.top

PHP:  public / protected / private
来源：http://llv.havefunace.top

JS:   #private 字段；其余公开
来源：http://aqi.nanxuanxn.top

TS:   public / protected / private
来源：http://xns.sweek.top

Java: public / protected / private / 默认包级
来源：http://aev.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rfw.yfazqb.com

Ruby: public / protected / private
来源：http://gqv.andypj.xyz

C#:   public / protected / private / internal
来源：http://mhq.jianghu66.top

[G11] getter / setter
来源：http://ctb.tanke756.top

Py:   @property 与 @x.setter
来源：http://eje.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wyg.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://wdc.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://hrr.snrcjt.cn

Java: public String getName() { return name; }
来源：http://gzc.jinqigfzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://atv.fzhhl.top

Ruby: attr_accessor :name
来源：http://hyy.c1oappe.top

C#:   public string Name { get; set; }
来源：http://uhv.smart0.xyz

[G12] 对象转字符串
来源：http://zas.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://ixh.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fmd.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://wxc.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://zjk.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://syl.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hbg.fktsv.cn

Ruby: def to_s; @name; end
来源：http://umu.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://djc.cucudq.cn

[G13] 判断对象类型
来源：http://lwe.svipenyu.cn

Py:   isinstance(u, User)
来源：http://qae.zdbjq.cn

PHP:  $u instanceof User
来源：http://gqp.yj20258888.top

JS:   u instanceof User
来源：http://svj.zdbjq.cn

TS:   u instanceof User
来源：http://coq.jinghuilouyu.cn

Java: u instanceof User
来源：http://amf.iojbl.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nle.epnwcf.com

Ruby: u.is_a?(User)
来源：http://nzb.yj202588.top

C#:   u is User
来源：http://pgl.gotoacloud.top

[G14] 数据类 / record
来源：http://bsg.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uuy.jqgufenzy.top

PHP:  // 用 readonly 属性模拟
来源：http://xtt.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://prd.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://gom.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://rmc.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://cuh.smart0.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fjh.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://ydt.ivvv.top

[G15] 枚举
来源：http://aap.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yrc.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cxv.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kgm.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ofo.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://inq.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tyt.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://mhd.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pal.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://khz.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vqy.havefunace.top

PHP:  get_object_vars($obj);
来源：http://jjs.bbcook.cn

JS:   Object.entries(obj)
来源：http://vpc.xinyue.icu

TS:   Object.entries(obj)
来源：http://wex.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gzo.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cpp.chenlongwang.top

Ruby: obj.instance_variables
来源：http://vxl.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://ktu.hywenlv.cn

================================================================================
来源：http://mwd.fanxiaobao.xyz

H. 异常与错误处理
来源：http://pjb.xuanzx.com

================================================================================
来源：http://gcr.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://kap.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yyd.aizwys.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dtv.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tax.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wvx.svipenyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zvd.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xkg.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xgl.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://goc.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://dcq.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hwb.ppjwa.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ztb.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uut.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://qbv.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ywk.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kmq.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kug.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wfo.fehbvm.com

[H03] 主动抛出异常
来源：http://tdr.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://tse.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://miu.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://nkr.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://xsd.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rqg.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eif.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://tjb.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://udd.svipenyu.cn

[H04] 自定义异常类型
来源：http://jxn.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://ize.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://djy.aizwys.cn

JS:   class MyError extends Error {}
来源：http://unc.birdmap.top

TS:   class MyError extends Error {}
来源：http://kbt.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://ytw.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bia.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://mun.uphjek.com

C#:   class MyException : Exception {}
来源：http://fpj.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://bme.yj202588.top

Py:   except ValueError as e:
来源：http://zbs.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://luc.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://qje.jqgfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://kzs.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://sul.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zxl.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://rnw.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bsi.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://fbo.meibo888.top

Py:   value = d.get("k") or default
来源：http://tni.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jaf.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://mje.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lpl.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://glm.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cmk.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://zql.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://rlj.tanke756.top

[H07] 断言
来源：http://cyk.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://sbl.chenzaomai.com

PHP:  assert($x > 0);
来源：http://zmw.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://upt.guannengcc.top

TS:   console.assert(x > 0);
来源：http://uxl.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://duw.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gjy.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://cen.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://atd.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://lre.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://dbq.fengsongda.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://osi.xylfe.cn

JS:   e.message;  e.stack
来源：http://akp.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hya.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gcx.9152youxi.cn

Go:   err.Error()
来源：http://mwb.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://ckc.svipenyu.cn

C#:   e.Message;  e.StackTrace
来源：http://cdc.tanke756.top

[H09] 带错误码的异常
来源：http://nkr.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yns.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ktt.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jyn.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hzu.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vzq.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vng.jlsjyb.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gxw.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ggc.shzxlz.cn

[H10] 资源自动释放
来源：http://hsm.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bng.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uie.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mpg.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rps.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ycu.shuidangran.top

Go:   defer f.Close()
来源：http://nnk.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wyg.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://siu.jianghu66.top

================================================================================
来源：http://syi.ybcxt.top

I. 正则表达式
来源：http://jmk.tanke756.top

================================================================================
来源：http://bhj.yj202588.top

[I01] 判断是否匹配
来源：http://ayf.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wjm.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://xfx.ivvv.top

JS:   /\d+/.test(s)
来源：http://hoh.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://fvw.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nyq.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gps.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://vcn.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://whg.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://dvr.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://int.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jjn.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ihi.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://ipd.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://flm.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gae.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://veu.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rgg.fengsongda.top

[I03] 提取捕获分组
来源：http://vqp.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iqo.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://drs.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qth.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rbj.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xxp.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jaa.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qwd.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jxj.ivvv.top

[I04] 正则替换
来源：http://nlh.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gfz.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uyx.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://fse.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ife.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://xal.ydjk.org.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://shl.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://clt.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rhm.quarkkingdee.top

[I05] 按正则拆分
来源：http://ryf.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aba.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wji.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://rtx.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://vkk.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://vay.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wtf.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://glk.mhx1999.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://put.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xni.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iqu.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://opc.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://boq.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkz.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tyg.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://usp.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gjj.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kju.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://pfq.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://njv.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://klf.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tgs.gogol.net.cn

TS:   /error/gim
来源：http://klr.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ygh.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iiy.sweek.top

Ruby: s.scan(/error/i)
来源：http://und.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dgz.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://xcj.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://okj.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://svq.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eaq.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wqr.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dyn.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tyw.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gjk.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://grk.52xcode.cn

================================================================================
来源：http://ddx.hongshengwenyu.top

J. 日期与时间
来源：http://nrg.xylfe.cn

================================================================================
来源：http://jwk.jqgfzy.top

[J01] 获取当前时间
来源：http://hdn.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wil.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://psq.redwolf501.top

JS:   new Date();  Date.now()
来源：http://llf.andypj.xyz

TS:   new Date();  Date.now()
来源：http://txm.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hue.c1oappe.top

Go:   time.Now()
来源：http://iwp.zhoulong.xyz

Ruby: Time.now
来源：http://tpv.jqgufenzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kpa.ybcxt.top

[J02] 格式化输出
来源：http://pvp.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gjs.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eju.dashuyun.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gzt.havefunace.top

TS:   d.toISOString()
来源：http://ufg.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kmi.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ani.haohaochexian.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ius.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ltg.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://kwx.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hsv.uphjek.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aaz.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://oqe.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://imp.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jvg.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hqn.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://bif.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pgn.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://vru.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pei.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wlc.yj20258888.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lbe.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://epv.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vbp.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lld.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vru.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yrl.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://kvs.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://dof.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://tri.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qdh.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qko.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://iob.hesvh.cn


<!-- 参考信息 -->