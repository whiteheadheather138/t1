代发 wailian999

Ruby: super
来源：http://ehu.gzhubu.top

C#:   base.Greet();
来源：http://bgv.chenzaomai.com

[G08] 静态方法与属性
来源：http://uyt.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pea.yj20258888.top

PHP:  public static function f() {}
来源：http://ype.andypj.xyz

JS:   static f() {}
来源：http://bea.xuetiantiany.cn

TS:   static f(): void {}
来源：http://yah.wangdashe.top

Java: static void f() {}
来源：http://gsm.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://brb.316326.xyz

Ruby: def self.f; end
来源：http://rmc.bbcook.cn

C#:   public static void F() {}
来源：http://kev.cucudq.cn

[G09] 接口 / 抽象类
来源：http://jtl.snrcjt.cn

Py:   from abc import ABC, abstractmethod
来源：http://oku.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zys.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://spi.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://eeh.hammf.cn

Java: interface Shape { double area(); }
来源：http://nca.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://ero.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gum.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://wlx.jinqigfzy.top

[G10] 访问控制
来源：http://wga.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://vpf.meibo888.top

PHP:  public / protected / private
来源：http://vuc.cashguo.top

JS:   #private 字段；其余公开
来源：http://jpd.daria6918.cn

TS:   public / protected / private
来源：http://ixk.cheryme.top

Java: public / protected / private / 默认包级
来源：http://wrj.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lxt.ybcxt.top

Ruby: public / protected / private
来源：http://wbb.havefunace.top

C#:   public / protected / private / internal
来源：http://psi.hesvh.cn

[G11] getter / setter
来源：http://sse.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://icf.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://spv.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://wyp.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://dmp.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://che.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sao.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://ipk.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://jep.0kj1m.cn

[G12] 对象转字符串
来源：http://lzk.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://tva.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://evd.ybcxt.top

JS:   toString() { return this.name; }
来源：http://uhk.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://ull.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://ugz.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://ipi.yongpay.top

Ruby: def to_s; @name; end
来源：http://mak.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://yqz.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://xtf.hysaishi.cn

Py:   isinstance(u, User)
来源：http://mmf.xylfe.cn

PHP:  $u instanceof User
来源：http://iqy.pycfn.com

JS:   u instanceof User
来源：http://cfv.feifeiyinyue.top

TS:   u instanceof User
来源：http://szr.zhongyouzk.top

Java: u instanceof User
来源：http://aso.shanyushiyangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lkb.wangshuangyany.cn

Ruby: u.is_a?(User)
来源：http://vqs.yj20258888.top

C#:   u is User
来源：http://gjy.sufxvd.cn

[G14] 数据类 / record
来源：http://kai.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ynf.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://jjq.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://syi.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://jvb.yueranfly.top

Java: record User(String name, int age) {}
来源：http://ckd.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://aig.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mdp.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://vxz.smart0.xyz

[G15] 枚举
来源：http://hmw.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gnn.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vfm.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zti.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fdz.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://czw.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ehp.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://ojb.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://taw.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://kdd.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jgz.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://hbg.daria6918.cn

JS:   Object.entries(obj)
来源：http://yqi.gzhubu.top

TS:   Object.entries(obj)
来源：http://vrm.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lbo.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wwm.jqgufenzy.top

Ruby: obj.instance_variables
来源：http://cvm.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://rom.wangshuangyany.cn

================================================================================
来源：http://pez.tanke756.top

H. 异常与错误处理
来源：http://skh.hcnkem.com

================================================================================
来源：http://cje.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://obq.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://svy.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ura.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ilz.shuidangran.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kon.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwm.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rjq.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bsa.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gsv.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://vid.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://rgp.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://agn.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://khl.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jsb.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wyo.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gzz.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://oti.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pqn.ydzc1.top

[H03] 主动抛出异常
来源：http://lut.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://zug.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dvh.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://uim.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://bpf.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://aoa.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pvk.quarkkingdee.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fem.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://xza.sjlbkw.cn

[H04] 自定义异常类型
来源：http://das.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://twk.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://ntc.shuidangran.top

JS:   class MyError extends Error {}
来源：http://ovx.jinghuilouyu.cn

TS:   class MyError extends Error {}
来源：http://tua.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://lgi.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wvb.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://lvp.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://qxl.fzhhl.top

[H05] 捕获特定类型
来源：http://xhv.zycfv.cn

Py:   except ValueError as e:
来源：http://rbm.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nxm.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://oey.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://woi.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://jqj.jinqigufen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fxl.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://xzy.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iaa.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://zap.c1oappe.top

Py:   value = d.get("k") or default
来源：http://uzg.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://ful.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://odx.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://asu.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://haj.sysykeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://idh.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://dut.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://ynu.xylfe.cn

[H07] 断言
来源：http://fmc.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://fxc.aizwys.cn

PHP:  assert($x > 0);
来源：http://tow.hcnkem.com

JS:   console.assert(x > 0);
来源：http://zxz.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://wib.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://bwd.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://adf.shanyushiyangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://vdb.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://rsz.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://viq.vqdsnc.cn

Py:   str(e);  traceback.format_exc()
来源：http://twj.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tkt.xuetiantiany.cn

JS:   e.message;  e.stack
来源：http://von.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hyz.snrcjt.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tkj.ydzc1.top

Go:   err.Error()
来源：http://upz.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://etv.jqgufenzy.top

C#:   e.Message;  e.StackTrace
来源：http://zhy.xylfe.cn

[H09] 带错误码的异常
来源：http://ocf.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zti.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wac.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rzp.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://skp.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zrq.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qib.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://vpe.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ivh.zhoulong.xyz

[H10] 资源自动释放
来源：http://tvd.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nlu.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vrk.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mnk.xuanzx.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ika.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ysd.cdnleiting.top

Go:   defer f.Close()
来源：http://rhk.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fiq.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aqq.aizwys.cn

================================================================================
来源：http://uhy.jqgufenzy.top

I. 正则表达式
来源：http://ory.gzhubu.top

================================================================================
来源：http://uyj.mhx1999.top

[I01] 判断是否匹配
来源：http://deg.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kcj.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://uri.smart0.xyz

JS:   /\d+/.test(s)
来源：http://liz.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://cyh.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yvi.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://raw.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://ixt.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gnt.xuanzx.com

[I02] 提取所有匹配
来源：http://ngw.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://iqk.nwbrower.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vmw.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vzj.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://xbb.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uvc.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qjr.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://xvx.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://glu.meibo888.top

[I03] 提取捕获分组
来源：http://crj.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gwx.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hvv.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ljv.wangdashe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zex.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://akp.daxiang520.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://thm.yueranfly.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rpp.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kax.chenjidiqi.icu

[I04] 正则替换
来源：http://rrv.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://sqw.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wfp.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ped.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://mqy.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://nib.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hnt.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kmx.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://agb.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://cjv.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ruw.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yos.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://yxn.yj20258.top

TS:   s.split(/\s*,\s*/)
来源：http://zbu.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://xwb.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aqp.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://rzy.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ldr.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qfd.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ssy.cqqwz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xqp.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://asm.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vbc.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fub.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ivb.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nyb.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eeg.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://mzg.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mdb.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uak.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lid.sysykeji.top

TS:   /error/gim
来源：http://ufi.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zsh.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tyn.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://dfj.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ghb.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://rkh.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xlp.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sdr.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qao.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rhz.havefunace.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dia.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eoh.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://npw.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dem.gotoacloud.top

================================================================================
来源：http://cwy.havefunace.top

J. 日期与时间
来源：http://kbm.tianlin.xyz

================================================================================
来源：http://iiz.yj20258.top

[J01] 获取当前时间
来源：http://wyk.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jbn.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fzd.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://xca.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://crw.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tos.guowangkeji.top

Go:   time.Now()
来源：http://mhp.smart0.xyz

Ruby: Time.now
来源：http://hko.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://krp.xziqi.cn

[J02] 格式化输出
来源：http://asn.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ejh.zhoulong.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://izx.zdbjq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pqd.dashuyun.cn

TS:   d.toISOString()
来源：http://sqs.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fkl.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gns.sweek.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lec.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fej.birdmap.top

[J03] 字符串解析为日期
来源：http://mpa.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ods.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jrh.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://nka.yongpay.top

TS:   new Date("2024-01-02")
来源：http://ekb.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://ucj.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gvs.ivvv.top

Ruby: Date.parse("2024-01-02")
来源：http://chr.jianghu66.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ggq.iojbl.cn

[J04] 时间戳与日期互转
来源：http://iar.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jbn.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cgq.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://usl.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ujd.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xrt.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eyi.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qgs.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ila.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://mjl.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://byx.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ryy.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cjm.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://etk.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://wlz.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ptc.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://oyz.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://uqb.aizwys.cn

[J06] 计算两时间之差
来源：http://jvn.mhx1999.top


<!-- 参考信息 -->