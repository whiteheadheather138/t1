代发 wailian999

JS:   super.greet();
来源：http://iyp.jinghuilouyu.cn

TS:   super.greet();
来源：http://cpb.hysaishi.cn

Java: super.greet();
来源：http://gqu.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ggk.gzhubu.top

Ruby: super
来源：http://rdi.smart0.xyz

C#:   base.Greet();
来源：http://nit.cashguo.top

[G08] 静态方法与属性
来源：http://ncc.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tre.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://fau.pengpengdd.cyou

JS:   static f() {}
来源：http://nmt.shangyingyoupin.top

TS:   static f(): void {}
来源：http://sac.jlsjyb.cn

Java: static void f() {}
来源：http://zqj.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mnx.yonumen.top

Ruby: def self.f; end
来源：http://qkl.tanke756.top

C#:   public static void F() {}
来源：http://sfx.hcnkem.com

[G09] 接口 / 抽象类
来源：http://wcd.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://rfa.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hyu.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bjx.chenzaomai.com

TS:   interface Shape { area(): number; }
来源：http://lvi.nwbrower.top

Java: interface Shape { double area(); }
来源：http://dpe.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://cby.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mkh.0kj1m.cn

C#:   interface IShape { double Area(); }
来源：http://iit.yuxming.cn

[G10] 访问控制
来源：http://juj.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://ilp.ehwqpu.com

PHP:  public / protected / private
来源：http://vtr.sysykeji.top

JS:   #private 字段；其余公开
来源：http://ehb.yangfankeji.com

TS:   public / protected / private
来源：http://lkd.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://jlt.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://akr.zhongyouzk.top

Ruby: public / protected / private
来源：http://uxb.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://hxr.andypj.xyz

[G11] getter / setter
来源：http://djz.sxryk.cn

Py:   @property 与 @x.setter
来源：http://wes.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bhw.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://obk.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://eig.gzhubu.top

Java: public String getName() { return name; }
来源：http://jke.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://inp.svipenyu.cn

Ruby: attr_accessor :name
来源：http://jkq.hcnkem.com

C#:   public string Name { get; set; }
来源：http://vbn.ydjk.org.cn

[G12] 对象转字符串
来源：http://pza.feifeiyinyue.top

Py:   def __str__(self): return self.name
来源：http://wui.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uoy.hesvh.cn

JS:   toString() { return this.name; }
来源：http://rwq.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://dyj.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://kzk.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://jki.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://vgf.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://ibg.fzhhl.top

[G13] 判断对象类型
来源：http://hxq.jyoumei.cn

Py:   isinstance(u, User)
来源：http://lwu.vehdjk.com

PHP:  $u instanceof User
来源：http://ixg.c1oappe.top

JS:   u instanceof User
来源：http://itc.smart0.xyz

TS:   u instanceof User
来源：http://yud.pengpengdd.cyou

Java: u instanceof User
来源：http://qmk.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ybk.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://rla.fengsongda.top

C#:   u is User
来源：http://epi.daxiang520.top

[G14] 数据类 / record
来源：http://jzf.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lto.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://lwv.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ocl.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://ojt.yueranfly.top

Java: record User(String name, int age) {}
来源：http://bkt.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://rsq.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ixo.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://prv.316326.xyz

[G15] 枚举
来源：http://dwk.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dhl.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nvi.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jdx.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tnp.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://shg.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vrt.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://sij.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ovz.yj202588.top

[G16] 对象转数组 / 字典
来源：http://utg.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nkf.meibo888.top

PHP:  get_object_vars($obj);
来源：http://iip.yueranfly.top

JS:   Object.entries(obj)
来源：http://kij.chenlongwang.top

TS:   Object.entries(obj)
来源：http://ria.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fxr.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wdm.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://npy.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://qzg.nanxuanxn.top

================================================================================
来源：http://oqq.0kj1m.cn

H. 异常与错误处理
来源：http://ryd.chenjidiqi.icu

================================================================================
来源：http://nml.vehdjk.com

[H01] try / catch 基础
来源：http://dcq.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://flp.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dfo.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vnl.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hvk.jinqigufen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lto.zdbjq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jeu.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qik.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://znu.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://czh.kuanghao11.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ljd.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ndy.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://lwh.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://umj.c1oappe.top

Java: try { f(); } finally { cleanup(); }
来源：http://psg.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://zoh.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://blk.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bpf.zhoulong.xyz

[H03] 主动抛出异常
来源：http://eit.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://umf.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ncq.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://mek.c1oappe.top

TS:   throw new Error("错误信息");
来源：http://fnz.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zce.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gmy.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wmr.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lma.jinqigfzy.top

[H04] 自定义异常类型
来源：http://koq.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://gps.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://kyw.wangdashe.top

JS:   class MyError extends Error {}
来源：http://sch.ydzc1.top

TS:   class MyError extends Error {}
来源：http://bkf.yonumen.top

Java: class MyException extends RuntimeException {}
来源：http://lcr.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tuy.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://fam.bbcook.cn

C#:   class MyException : Exception {}
来源：http://eyj.mhx1999.top

[H05] 捕获特定类型
来源：http://ijl.shuidangran.top

Py:   except ValueError as e:
来源：http://hee.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vfx.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://lto.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://oaf.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://rlw.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hvd.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://fve.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mft.tanke756.top

[H06] 可选值 / 空值安全访问
来源：http://kur.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://prv.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pbd.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://iku.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://dne.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eli.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eyp.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://vte.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://jxw.birdmap.top

[H07] 断言
来源：http://eyg.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://qxx.hammf.cn

PHP:  assert($x > 0);
来源：http://szr.cashguo.top

JS:   console.assert(x > 0);
来源：http://fxz.c1oappe.top

TS:   console.assert(x > 0);
来源：http://rff.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://dyr.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qyj.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://rbi.meibo888.top

C#:   Debug.Assert(x > 0);
来源：http://sla.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://ptf.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://auz.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yva.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://hbo.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://oub.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://nie.birdmap.top

Go:   err.Error()
来源：http://lqa.hysaishi.cn

Ruby: e.message;  e.backtrace
来源：http://dcc.bbcook.cn

C#:   e.Message;  e.StackTrace
来源：http://kyj.tanke756.top

[H09] 带错误码的异常
来源：http://knp.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yju.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://maw.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://joz.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lmd.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lwk.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rhu.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://taj.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yuc.52xcode.cn

[H10] 资源自动释放
来源：http://rsa.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://tfc.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://euo.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqr.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fsj.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://glm.bjfxy.top

Go:   defer f.Close()
来源：http://exr.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cnr.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pst.jqgfzy.top

================================================================================
来源：http://lkb.shzxlz.cn

I. 正则表达式
来源：http://yvc.fehbvm.com

================================================================================
来源：http://rth.zhijiandao.cn

[I01] 判断是否匹配
来源：http://gnh.0kj1m.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hff.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uuo.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://azz.hammf.cn

TS:   /\d+/.test(s)
来源：http://tkv.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sws.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wfg.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://mhd.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ons.hnxiangtu.top

[I02] 提取所有匹配
来源：http://ewv.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://rkp.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pnc.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cag.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://occ.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://czw.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rra.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://ueq.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://unr.vqdsnc.cn

[I03] 提取捕获分组
来源：http://gid.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ttz.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sto.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xhr.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vtc.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nsk.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nwx.meibo888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xyy.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kpd.cucudq.cn

[I04] 正则替换
来源：http://zlj.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rdj.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hkk.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://ozp.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://zgo.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://yrf.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ndl.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://okq.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qzy.hammf.cn

[I05] 按正则拆分
来源：http://vxo.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://gdp.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uzv.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://nuy.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://huq.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://xmm.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rjd.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ish.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://okp.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tmr.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sui.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hhj.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hvj.shangyingyoupin.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oir.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iub.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vyi.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lgo.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://znd.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://crf.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uhu.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://swt.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mcz.yonumen.top

TS:   /error/gim
来源：http://wxq.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://prw.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tfu.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://xhh.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hzm.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://tvp.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oro.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iyx.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwu.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nch.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://esh.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ycc.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qhs.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ztf.316326.xyz

================================================================================
来源：http://nzb.vqdsnc.cn

J. 日期与时间
来源：http://fif.nwbrower.top

================================================================================
来源：http://vqb.shzxlz.cn

[J01] 获取当前时间
来源：http://wss.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hmb.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://djf.fehbvm.com

JS:   new Date();  Date.now()
来源：http://yxp.yj202588.top

TS:   new Date();  Date.now()
来源：http://njw.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bjt.zhaomingkeji.xyz

Go:   time.Now()
来源：http://ncy.sufxvd.cn

Ruby: Time.now
来源：http://jvd.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wza.yj202588.top

[J02] 格式化输出
来源：http://wqp.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nvj.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bbh.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xfq.dianchejie.cn

TS:   d.toISOString()
来源：http://jnz.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lxz.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xiu.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kov.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uvo.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://ile.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qpk.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gfb.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://pwt.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://ypm.jinqigfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://yfh.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nkl.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://zpy.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mdt.fzhhl.top

[J04] 时间戳与日期互转
来源：http://hma.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://woi.gzhubu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bii.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nqa.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://piu.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://spc.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://crq.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hlk.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://smq.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://dvz.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://pck.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vlc.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sah.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bpc.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://dlk.jianghu66.top


<!-- 参考信息 -->