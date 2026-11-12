代发 wailian999

JS:   super.greet();
来源：http://sxc.fktsv.cn

TS:   super.greet();
来源：http://rvb.aibaodan.cn

Java: super.greet();
来源：http://kdw.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fbi.hysaishi.cn

Ruby: super
来源：http://afa.aibaodan.cn

C#:   base.Greet();
来源：http://miu.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://wws.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fjc.smart0.xyz

PHP:  public static function f() {}
来源：http://apk.gogol.net.cn

JS:   static f() {}
来源：http://uwj.gzhubu.top

TS:   static f(): void {}
来源：http://svp.fengsongda.top

Java: static void f() {}
来源：http://eaj.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uqk.zhijiandao.cn

Ruby: def self.f; end
来源：http://jtl.guannengcc.top

C#:   public static void F() {}
来源：http://kjs.sysykeji.top

[G09] 接口 / 抽象类
来源：http://ivz.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://pia.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://vds.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tfd.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://uzo.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://pbo.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://gts.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mqf.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://wuo.fktsv.cn

[G10] 访问控制
来源：http://ddm.ybcxt.top

Py:   约定 _protected / __private（不强制）
来源：http://kim.jinqigufen.top

PHP:  public / protected / private
来源：http://gls.wangdashe.top

JS:   #private 字段；其余公开
来源：http://jua.meibo888.top

TS:   public / protected / private
来源：http://vot.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://ezt.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vbs.vqdsnc.cn

Ruby: public / protected / private
来源：http://kju.guowangkeji.top

C#:   public / protected / private / internal
来源：http://ejy.xuetiantiany.cn

[G11] getter / setter
来源：http://ywd.yj20258.top

Py:   @property 与 @x.setter
来源：http://lzb.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ftq.yj20258.top

JS:   get name() { return this._name; }
来源：http://iiw.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://zyo.redwolf501.top

Java: public String getName() { return name; }
来源：http://cdk.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://gbk.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://zcp.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://mhi.dashuyun.cn

[G12] 对象转字符串
来源：http://gop.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://img.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://zoy.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://omq.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://fcs.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://who.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://tes.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://ovn.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://oyh.9152youxi.cn

[G13] 判断对象类型
来源：http://ubw.yvedp.cn

Py:   isinstance(u, User)
来源：http://pnz.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://inb.hongshengwenyu.top

JS:   u instanceof User
来源：http://nnf.jianghu66.top

TS:   u instanceof User
来源：http://oha.ivvv.top

Java: u instanceof User
来源：http://lpw.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ojf.ybcxt.top

Ruby: u.is_a?(User)
来源：http://xqi.hongshengwenyu.top

C#:   u is User
来源：http://bjf.yvedp.cn

[G14] 数据类 / record
来源：http://gtq.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://egt.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://zrr.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ndb.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://fla.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://nww.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://ykg.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pmo.tanke756.top

C#:   record User(string Name, int Age);
来源：http://lug.aizwys.cn

[G15] 枚举
来源：http://ikj.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hpt.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://utu.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mky.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://llk.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://qdq.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gur.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://dqq.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://guc.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://smy.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gkr.hammf.cn

PHP:  get_object_vars($obj);
来源：http://vsk.yj20258.top

JS:   Object.entries(obj)
来源：http://hvj.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://ewc.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gnv.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cbg.yangfankeji.com

Ruby: obj.instance_variables
来源：http://qfd.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://crb.ydjk.org.cn

================================================================================
来源：http://vge.gotoacloud.top

H. 异常与错误处理
来源：http://ico.fengsongda.top

================================================================================
来源：http://oqv.hnqzz.top

[H01] try / catch 基础
来源：http://jlv.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://frm.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uyz.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vmi.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xod.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://raz.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gyt.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ooy.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wfh.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://cei.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aic.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cob.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://swo.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fgt.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://knl.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wlq.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ksj.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xem.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://bbb.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://exe.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oun.yonumen.top

JS:   throw new Error("错误信息");
来源：http://ubo.yanxiufei.cn

TS:   throw new Error("错误信息");
来源：http://tpd.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://brm.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hxx.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hgk.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://epf.mhx1999.top

[H04] 自定义异常类型
来源：http://lds.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://qsl.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://dhf.meibo888.top

JS:   class MyError extends Error {}
来源：http://jwg.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://amt.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://wio.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qop.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://ejd.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://pra.gotoacloud.top

[H05] 捕获特定类型
来源：http://ywd.chenzaomai.com

Py:   except ValueError as e:
来源：http://pem.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dag.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://yad.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://jpt.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://wpc.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ezf.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://zbg.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uku.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://uot.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://rpa.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dvw.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://xht.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lnr.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xnk.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hct.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://ezf.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://onk.chenzaomai.com

[H07] 断言
来源：http://dmy.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://rtw.tianlin.xyz

PHP:  assert($x > 0);
来源：http://nnc.zhongyouzk.top

JS:   console.assert(x > 0);
来源：http://dtn.wangdashe.top

TS:   console.assert(x > 0);
来源：http://dcx.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://qul.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://les.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gya.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://num.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://byq.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://hxs.bbcook.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://taa.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://uqd.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://snc.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://emv.ydzc1.top

Go:   err.Error()
来源：http://obz.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://cjq.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://vzi.havefunace.top

[H09] 带错误码的异常
来源：http://gvk.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kbg.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vki.gzhubu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://drw.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cgj.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tec.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sxy.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bpd.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gwy.ctjpmb.com

[H10] 资源自动释放
来源：http://bks.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nxg.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mgd.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bmo.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://osc.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://urw.bbcook.cn

Go:   defer f.Close()
来源：http://dcx.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mlw.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://urz.hnqzz.top

================================================================================
来源：http://vpd.9152youxi.cn

I. 正则表达式
来源：http://yrm.svipenyu.cn

================================================================================
来源：http://vfh.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://wzr.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xbv.chenlongwang.top

PHP:  preg_match('/\d+/', $s);
来源：http://pmp.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://xpn.c1oappe.top

TS:   /\d+/.test(s)
来源：http://krb.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pna.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uyz.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://sef.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uui.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://pbc.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://hrj.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ytb.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dpz.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://snr.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hhs.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nvt.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://rjx.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbb.epnwcf.com

[I03] 提取捕获分组
来源：http://uvi.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rry.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xct.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wll.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uel.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hen.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oox.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gfz.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lan.zycfv.cn

[I04] 正则替换
来源：http://dsw.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qnl.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://igh.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://eax.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vhc.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://tek.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nyj.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uqt.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wzl.nanxuanxn.top

[I05] 按正则拆分
来源：http://dje.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rpp.yongpay.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://isi.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://pkc.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://oqk.hywenlv.cn

Java: s.split("\\s*,\\s*")
来源：http://cfw.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lfl.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://zng.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ngx.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nww.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://upb.snrcjt.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iqn.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yez.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fhn.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jyo.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rmj.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gqs.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bsy.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://ozz.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yei.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dpu.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kju.shzxlz.cn

TS:   /error/gim
来源：http://ebq.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ech.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://anl.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://ygf.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://quz.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://vxq.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zkp.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zea.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xpl.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fpz.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehb.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hsn.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cwn.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pxo.ydjk.org.cn

================================================================================
来源：http://oik.jqgfzy.top

J. 日期与时间
来源：http://npb.jqgufenzy.top

================================================================================
来源：http://eem.yuxming.cn

[J01] 获取当前时间
来源：http://tsb.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uqr.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gas.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://yow.yj202588.top

TS:   new Date();  Date.now()
来源：http://ktx.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aul.hysaishi.cn

Go:   time.Now()
来源：http://opw.gzhubu.top

Ruby: Time.now
来源：http://srq.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://osr.ehwqpu.com

[J02] 格式化输出
来源：http://luw.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ibs.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://agd.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://chz.tianlin.xyz

TS:   d.toISOString()
来源：http://eui.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fzk.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://muy.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sxh.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ikv.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://iut.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://thm.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ysb.cheryme.top

JS:   new Date("2024-01-02")
来源：http://gsk.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://hbb.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fsp.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fri.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://oxs.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://voq.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://vxc.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://adk.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qfe.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mev.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yaz.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rzk.jinqigfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sln.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tns.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bjj.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://lfx.chenzaomai.com

Py:   now + timedelta(days=7)
来源：http://qrx.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://yhi.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbw.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpt.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://tkc.zhiwuduotai.top


<!-- 参考信息 -->