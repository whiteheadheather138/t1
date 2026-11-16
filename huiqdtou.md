代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://mxy.jiagoushi.top

[G07] 调用父类方法
来源：http://hgu.yuanzhike.top

Py:   super().greet()
来源：http://aka.0kj1m.cn

PHP:  parent::greet();
来源：http://hfx.shangyingyoupin.top

JS:   super.greet();
来源：http://jpl.yj20258.top

TS:   super.greet();
来源：http://xov.zycfv.cn

Java: super.greet();
来源：http://xms.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wix.wangshuangyany.cn

Ruby: super
来源：http://ynv.jyoumei.cn

C#:   base.Greet();
来源：http://ksm.gogol.net.cn

[G08] 静态方法与属性
来源：http://qdb.aizwys.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://keo.gotoacloud.top

PHP:  public static function f() {}
来源：http://llo.gaohongyu789.top

JS:   static f() {}
来源：http://pfs.yj20258888.top

TS:   static f(): void {}
来源：http://wpw.hysaishi.cn

Java: static void f() {}
来源：http://uaq.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tnu.yongpay.top

Ruby: def self.f; end
来源：http://gxs.cqqwz.cn

C#:   public static void F() {}
来源：http://oov.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://byr.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://qeh.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hxy.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://obr.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://rmv.cashguo.top

Java: interface Shape { double area(); }
来源：http://wvr.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://eya.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://egq.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://kmi.hnxiangtu.top

[G10] 访问控制
来源：http://dlq.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://skp.yuanzhike.top

PHP:  public / protected / private
来源：http://jgk.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://zak.9152youxi.cn

TS:   public / protected / private
来源：http://xfo.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://soz.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vcs.zdbjq.cn

Ruby: public / protected / private
来源：http://xwz.wangdashe.top

C#:   public / protected / private / internal
来源：http://iwl.jqgufenzy.top

[G11] getter / setter
来源：http://myf.havefunace.top

Py:   @property 与 @x.setter
来源：http://roy.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://wpx.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://sia.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://twj.dashuyun.cn

Java: public String getName() { return name; }
来源：http://koi.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mbt.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://mzg.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://mga.andypj.xyz

[G12] 对象转字符串
来源：http://aeh.birdmap.top

Py:   def __str__(self): return self.name
来源：http://aks.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://evp.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://sgm.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://vwj.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://nvo.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kih.hcnkem.com

Ruby: def to_s; @name; end
来源：http://vpp.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://drc.uphjek.com

[G13] 判断对象类型
来源：http://ypj.zhixingplan.top

Py:   isinstance(u, User)
来源：http://osz.yonumen.top

PHP:  $u instanceof User
来源：http://dna.bjfxy.top

JS:   u instanceof User
来源：http://iys.guannengcc.top

TS:   u instanceof User
来源：http://ngk.xinyue.icu

Java: u instanceof User
来源：http://ilm.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oyo.pycfn.com

Ruby: u.is_a?(User)
来源：http://nxc.zhaomingkeji.xyz

C#:   u is User
来源：http://ofy.yanxiufei.cn

[G14] 数据类 / record
来源：http://epd.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zjo.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://wnv.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://zlm.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://wgd.hcnkem.com

Java: record User(String name, int age) {}
来源：http://fti.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://hjg.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vll.meibo888.top

C#:   record User(string Name, int Age);
来源：http://dha.zhongyouzk.top

[G15] 枚举
来源：http://erp.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gek.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://frg.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nct.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ulj.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://tmf.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tue.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://mjd.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vbh.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://laf.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oom.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://nzt.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://ebz.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://wtx.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cwa.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://phw.zdqjudy.top

Ruby: obj.instance_variables
来源：http://smq.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://muz.birdmap.top

================================================================================
来源：http://ufo.ppjwa.cn

H. 异常与错误处理
来源：http://ogq.gzhubu.top

================================================================================
来源：http://uvc.jianghu66.top

[H01] try / catch 基础
来源：http://kex.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://olw.bjfxy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nrx.andypj.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qfr.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zgy.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pid.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://twq.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vpx.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mki.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://fif.zdqjudy.top

Py:   try: f()⏎finally: cleanup()
来源：http://bdt.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jks.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zgf.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ofo.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://htb.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://sho.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pyg.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rtx.gotoacloud.top

[H03] 主动抛出异常
来源：http://nco.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://yil.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nmw.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://mgb.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://uyi.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ozf.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gkp.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xsn.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nqx.andypj.xyz

[H04] 自定义异常类型
来源：http://uhc.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://pfw.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bwv.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://lke.yueranfly.top

TS:   class MyError extends Error {}
来源：http://yaj.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://afz.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xqf.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://vxb.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://ihq.havefunace.top

[H05] 捕获特定类型
来源：http://mbk.hesvh.cn

Py:   except ValueError as e:
来源：http://bqu.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xou.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://ewm.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://alh.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://zhy.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ehd.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://obj.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vhc.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://zkh.yonumen.top

Py:   value = d.get("k") or default
来源：http://nyu.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hrw.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://anp.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tbh.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pff.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tlj.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://qnt.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://bbo.ywan-chungtsiang.top

[H07] 断言
来源：http://jfe.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://qow.xinyue.icu

PHP:  assert($x > 0);
来源：http://mbq.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://wua.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://bhq.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://xii.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uds.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://xbg.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://ihu.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://znw.gotoacloud.top

Py:   str(e);  traceback.format_exc()
来源：http://pnn.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ebf.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://zcc.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xay.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://gcc.shuidangran.top

Go:   err.Error()
来源：http://uzx.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://xsq.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://owz.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://vqc.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yyo.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jhm.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cqu.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jfw.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ucb.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fpe.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://lhy.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xnz.smart0.xyz

[H10] 资源自动释放
来源：http://fvy.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pbw.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://akt.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yse.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kpr.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rep.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://xkp.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://emd.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rmc.ehwqpu.com

================================================================================
来源：http://vpj.yuanzhike.top

I. 正则表达式
来源：http://asm.xuanzx.com

================================================================================
来源：http://cxv.nanxinkj.top

[I01] 判断是否匹配
来源：http://pfq.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uha.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://fau.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://asl.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://oqk.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://die.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eaq.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://smk.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iqp.316326.xyz

[I02] 提取所有匹配
来源：http://qit.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://nao.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vzw.52xcode.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://msc.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://xie.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zua.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kpn.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://wwg.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wpd.cucudq.cn

[I03] 提取捕获分组
来源：http://fbk.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://usb.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vyj.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jdk.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://juh.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://quk.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qel.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://abs.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dnh.daxiang520.top

[I04] 正则替换
来源：http://xkc.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://evv.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uap.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sco.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://dnq.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://lrs.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qag.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xpm.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hqt.cqqwz.cn

[I05] 按正则拆分
来源：http://eoo.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://soa.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sqi.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://nri.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://imi.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://tbm.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zfn.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://oaw.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wnm.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kym.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://edc.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ewf.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qjp.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ury.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://duj.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aen.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mus.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wvg.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://sgp.shuidangran.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ixb.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mli.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ryx.ydjk.org.cn

TS:   /error/gim
来源：http://kvr.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mzh.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blb.havefunace.top

Ruby: s.scan(/error/i)
来源：http://eqk.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pdx.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://mhi.zhaomingkeji.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ene.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zho.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mma.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wjj.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jko.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rct.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bfw.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://drz.aibaodan.cn

================================================================================
来源：http://kbk.cdnleiting.top

J. 日期与时间
来源：http://tgv.52xcode.cn

================================================================================
来源：http://ntb.sxryk.cn

[J01] 获取当前时间
来源：http://vmy.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hch.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gzy.xziqi.cn

JS:   new Date();  Date.now()
来源：http://lrx.yj20258888.top

TS:   new Date();  Date.now()
来源：http://qgx.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xzg.gotoacloud.top

Go:   time.Now()
来源：http://vkj.gogol.net.cn

Ruby: Time.now
来源：http://qtb.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lri.yangfankeji.com

[J02] 格式化输出
来源：http://kld.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vkq.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xvk.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sud.jinqigfzy.top

TS:   d.toISOString()
来源：http://bym.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://phc.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://szd.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gze.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://waw.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://wbg.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://imx.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wxe.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://edo.sweek.top

TS:   new Date("2024-01-02")
来源：http://inq.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zqd.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wus.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://xth.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://geq.vehdjk.com

[J04] 时间戳与日期互转
来源：http://rwc.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zrt.havefunace.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gir.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jtk.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fse.fehbvm.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://grd.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rrt.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wvu.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://waw.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://eba.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://vtv.xylfe.cn


<!-- 参考信息 -->