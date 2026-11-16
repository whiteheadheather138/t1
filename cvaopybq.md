代发 wailian999

Ruby: super
来源：http://sfu.hcnkem.com

C#:   base.Greet();
来源：http://iey.yuxming.cn

[G08] 静态方法与属性
来源：http://cnj.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cxg.zhixingplan.top

PHP:  public static function f() {}
来源：http://wti.ydjk.org.cn

JS:   static f() {}
来源：http://shb.hcnkem.com

TS:   static f(): void {}
来源：http://qkx.cdnleiting.top

Java: static void f() {}
来源：http://nkg.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://glo.quarkkingdee.top

Ruby: def self.f; end
来源：http://gdd.yangfankeji.com

C#:   public static void F() {}
来源：http://ctm.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://ahr.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://dej.cashguo.top

PHP:  interface Shape { public function area(): float; }
来源：http://tjq.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sqj.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://bhc.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://mqy.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://whi.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yhf.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://uke.sufxvd.cn

[G10] 访问控制
来源：http://lxe.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://zmf.yongpay.top

PHP:  public / protected / private
来源：http://zvy.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://ysu.dianchejie.cn

TS:   public / protected / private
来源：http://hlk.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://arj.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ebr.sjlbkw.cn

Ruby: public / protected / private
来源：http://zlw.9152youxi.cn

C#:   public / protected / private / internal
来源：http://vxc.xziqi.cn

[G11] getter / setter
来源：http://jkr.wangdashe.top

Py:   @property 与 @x.setter
来源：http://bpt.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bdg.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://cwm.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://lsl.wangdashe.top

Java: public String getName() { return name; }
来源：http://ota.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://jyy.tianlin.xyz

Ruby: attr_accessor :name
来源：http://ajo.meibo888.top

C#:   public string Name { get; set; }
来源：http://iby.jlsjyb.cn

[G12] 对象转字符串
来源：http://jbl.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://joh.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://bcc.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://gcl.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://eta.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://gff.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://jsn.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://bck.uphjek.com

C#:   public override string ToString() => Name;
来源：http://roo.yfazqb.com

[G13] 判断对象类型
来源：http://gdt.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://ajr.zdbjq.cn

PHP:  $u instanceof User
来源：http://jyo.pycfn.com

JS:   u instanceof User
来源：http://nhq.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://ufx.zhaomingkeji.xyz

Java: u instanceof User
来源：http://bdq.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ruc.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://iqo.dianchejie.cn

C#:   u is User
来源：http://alh.yuxming.cn

[G14] 数据类 / record
来源：http://lwm.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pgs.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://pzy.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yig.sweek.top

TS:   type User = { name: string; age: number };
来源：http://dyb.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://jxe.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://wky.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xff.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://wco.xingfuxueyuan.xyz

[G15] 枚举
来源：http://ipa.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://llr.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tky.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hya.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pmw.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://ukl.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://slj.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://fox.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gjo.pycfn.com

[G16] 对象转数组 / 字典
来源：http://cpe.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jtq.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://loc.gotoacloud.top

JS:   Object.entries(obj)
来源：http://uwn.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://qgx.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ong.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ehz.jiagoushi.top

Ruby: obj.instance_variables
来源：http://iuq.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://pad.jinqigufen.top

================================================================================
来源：http://adn.ivvv.top

H. 异常与错误处理
来源：http://stx.ctjpmb.com

================================================================================
来源：http://egv.gzhubu.top

[H01] try / catch 基础
来源：http://lbf.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jpv.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wch.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://syw.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pff.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ueu.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sry.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ssm.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zby.hesvh.cn

[H02] finally / ensure 收尾
来源：http://bup.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://wav.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ugx.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://sqs.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lve.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://rjj.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ntd.tarul.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nkv.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vso.daria6918.cn

[H03] 主动抛出异常
来源：http://hiv.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://vpq.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pgz.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://wdg.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://zqp.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lpm.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kqx.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pco.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://dse.ydzc1.top

[H04] 自定义异常类型
来源：http://gwq.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://big.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://obu.xuanzx.com

JS:   class MyError extends Error {}
来源：http://nzz.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://cxq.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://ubk.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://okn.fengsongda.top

Ruby: class MyError < StandardError; end
来源：http://zxa.hammf.cn

C#:   class MyException : Exception {}
来源：http://wfd.ivvv.top

[H05] 捕获特定类型
来源：http://pak.jqgfzy.top

Py:   except ValueError as e:
来源：http://hip.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qky.pengpengdd.cyou

JS:   if (e instanceof TypeError) {}
来源：http://exb.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://bsx.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://qsl.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://efz.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://nmw.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bmc.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://rfx.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://aob.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://dec.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://osa.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://odi.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bit.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dmb.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://dtj.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://qdk.wangshuangyany.cn

[H07] 断言
来源：http://ama.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://ngj.c1oappe.top

PHP:  assert($x > 0);
来源：http://msf.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://ria.pycfn.com

TS:   console.assert(x > 0);
来源：http://ptf.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://djr.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kdh.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hvh.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://vvr.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://ush.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://azm.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vqf.c1oappe.top

JS:   e.message;  e.stack
来源：http://utv.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cvv.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tpc.shuidangran.top

Go:   err.Error()
来源：http://zfz.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://dsm.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://njj.yuanzhike.top

[H09] 带错误码的异常
来源：http://cyw.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nya.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wck.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lmo.yj202588.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jcr.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ofz.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lld.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://otk.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ouq.yanxiufei.cn

[H10] 资源自动释放
来源：http://kkj.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://qwy.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://siu.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eae.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sbe.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eif.yangfankeji.com

Go:   defer f.Close()
来源：http://gjf.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xzz.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://get.ywan-chungtsiang.top

================================================================================
来源：http://dut.pycfn.com

I. 正则表达式
来源：http://qsq.tian-w.cn

================================================================================
来源：http://eyx.yongpay.top

[I01] 判断是否匹配
来源：http://swj.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://emk.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ayy.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://tiz.yfazqb.com

TS:   /\d+/.test(s)
来源：http://ejj.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gpk.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kcr.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://pqh.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jvp.zycfv.cn

[I02] 提取所有匹配
来源：http://nnp.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://ugm.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kfg.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qbo.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://gcp.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vlj.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xeo.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://wdh.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cem.hcnkem.com

[I03] 提取捕获分组
来源：http://jzh.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mjb.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cmo.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cax.sxryk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xzi.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xos.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tli.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wph.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pta.tarul.cn

[I04] 正则替换
来源：http://ity.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jtv.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rnn.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lkk.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://rbl.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://ezj.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yhq.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tpf.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sju.daxiang520.top

[I05] 按正则拆分
来源：http://ygq.316326.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://zdc.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aup.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://qix.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://qil.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://qdm.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jlr.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jjv.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kwu.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wlz.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://slr.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ywj.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ybp.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldm.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xog.dashuyun.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tbk.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://muh.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ceu.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://yso.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mjz.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sma.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dyj.tanke756.top

TS:   /error/gim
来源：http://qbs.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ois.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mmg.tanke756.top

Ruby: s.scan(/error/i)
来源：http://fag.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://olq.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://nsv.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aow.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qpm.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hsc.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://agh.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mgl.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://czh.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iwz.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://scs.daxiang520.top

================================================================================
来源：http://gzv.316326.xyz

J. 日期与时间
来源：http://ciw.sufxvd.cn

================================================================================
来源：http://xie.cucudq.cn

[J01] 获取当前时间
来源：http://wob.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cbr.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bmd.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://hrv.aizwys.cn

TS:   new Date();  Date.now()
来源：http://mfp.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zax.wangdashe.top

Go:   time.Now()
来源：http://rke.zycfv.cn

Ruby: Time.now
来源：http://rmu.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ghy.zhixingplan.top

[J02] 格式化输出
来源：http://ayp.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pwe.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kdb.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lqh.tarul.cn

TS:   d.toISOString()
来源：http://bko.yueranfly.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xmb.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dpa.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xjk.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uen.xuanzx.com

[J03] 字符串解析为日期
来源：http://qic.ppjwa.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ldx.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tst.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://amx.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://atz.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://gon.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://grq.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://jvt.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zwl.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://doq.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qmi.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mvt.c1oappe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qez.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yvt.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lpw.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vdj.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ksm.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fah.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://bmo.cheryme.top

Py:   now + timedelta(days=7)
来源：http://xep.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://olh.gaohongyu789.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gap.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqx.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://wxu.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xrq.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://ubi.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cmx.jiagoushi.top

[J06] 计算两时间之差
来源：http://ale.hysaishi.cn


<!-- 参考信息 -->