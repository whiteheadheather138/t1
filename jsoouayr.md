代发 wailian999

Ruby: super
来源：http://qjq.zhixingplan.top

C#:   base.Greet();
来源：http://gwu.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://mna.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hdv.tianlin.xyz

PHP:  public static function f() {}
来源：http://oms.shuidangran.top

JS:   static f() {}
来源：http://ejy.jianghu66.top

TS:   static f(): void {}
来源：http://fqd.meibo888.top

Java: static void f() {}
来源：http://moy.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vmr.hywenlv.cn

Ruby: def self.f; end
来源：http://joy.316326.xyz

C#:   public static void F() {}
来源：http://whn.yueranfly.top

[G09] 接口 / 抽象类
来源：http://zph.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://cyo.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://bgg.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://xjc.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://eow.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://kgn.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://mcr.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pgn.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://pww.birdmap.top

[G10] 访问控制
来源：http://yng.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://ljw.daxiang520.top

PHP:  public / protected / private
来源：http://gti.iojbl.cn

JS:   #private 字段；其余公开
来源：http://raf.yvedp.cn

TS:   public / protected / private
来源：http://joe.uphjek.com

Java: public / protected / private / 默认包级
来源：http://uby.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qlo.xuanzx.com

Ruby: public / protected / private
来源：http://boz.hammf.cn

C#:   public / protected / private / internal
来源：http://tho.ivvv.top

[G11] getter / setter
来源：http://zge.xinyue.icu

Py:   @property 与 @x.setter
来源：http://vjs.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xrz.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://rpq.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://zti.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://zwz.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fgh.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://rqk.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://nks.meibo888.top

[G12] 对象转字符串
来源：http://mlr.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://jzz.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cxr.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://afo.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://wyc.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://yol.jinqigfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://eof.sjlbkw.cn

Ruby: def to_s; @name; end
来源：http://zfq.jianghu66.top

C#:   public override string ToString() => Name;
来源：http://nok.316326.xyz

[G13] 判断对象类型
来源：http://ksr.cucudq.cn

Py:   isinstance(u, User)
来源：http://hpj.316326.xyz

PHP:  $u instanceof User
来源：http://caj.sjlbkw.cn

JS:   u instanceof User
来源：http://odg.chenlongwang.top

TS:   u instanceof User
来源：http://kbw.yfazqb.com

Java: u instanceof User
来源：http://ovf.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zak.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://rkf.xziqi.cn

C#:   u is User
来源：http://krx.yuxming.cn

[G14] 数据类 / record
来源：http://stf.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xoq.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://fgv.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://xcm.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://rzm.yongpay.top

Java: record User(String name, int age) {}
来源：http://dbr.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://jrs.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fev.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://wzt.dashuyun.cn

[G15] 枚举
来源：http://hiu.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dfi.bbcook.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ucn.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xcg.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tcj.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://zis.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gcv.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://vyf.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aos.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://pnq.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tka.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://tor.fktsv.cn

JS:   Object.entries(obj)
来源：http://vyl.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://kmn.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qqa.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wqj.mhx1999.top

Ruby: obj.instance_variables
来源：http://nan.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://fez.bjfxy.top

================================================================================
来源：http://dyj.mhx1999.top

H. 异常与错误处理
来源：http://gzn.tanke756.top

================================================================================
来源：http://xlu.ppjwa.cn

[H01] try / catch 基础
来源：http://fea.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wga.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dmm.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lgr.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zxw.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jsq.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ope.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mpe.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vmn.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://qxu.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://kjl.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eaf.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://icj.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sbh.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://dxj.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://apr.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jib.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://clv.svipenyu.cn

[H03] 主动抛出异常
来源：http://qsg.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://xoz.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lrm.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://qnv.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://ljc.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wiq.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wlg.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://icj.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uqm.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://ebu.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://vyj.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://hgg.zdqjudy.top

JS:   class MyError extends Error {}
来源：http://yfm.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://vkg.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://xhg.aizwys.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zue.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://wau.meibo888.top

C#:   class MyException : Exception {}
来源：http://zdl.jinqigfzy.top

[H05] 捕获特定类型
来源：http://fxc.bjfxy.top

Py:   except ValueError as e:
来源：http://dxb.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zpl.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://tmn.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://tsc.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://csq.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kqo.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://qrg.jqgfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kli.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://psl.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://ksw.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qwt.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://ock.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://elg.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pto.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cpq.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://alk.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://arf.yonumen.top

[H07] 断言
来源：http://dbr.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://gow.uphjek.com

PHP:  assert($x > 0);
来源：http://sdu.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://atd.havefunace.top

TS:   console.assert(x > 0);
来源：http://duo.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://ymd.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mvh.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://efq.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://moj.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://dlp.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://iiu.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jrt.zhengqikj.top

JS:   e.message;  e.stack
来源：http://bzs.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://yfq.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kys.jyoumei.cn

Go:   err.Error()
来源：http://lqu.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://plr.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://zan.yongpay.top

[H09] 带错误码的异常
来源：http://gma.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qil.yj20258.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://psg.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ndi.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tth.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dly.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xlb.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://qap.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://joi.jlsjyb.cn

[H10] 资源自动释放
来源：http://kej.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ksl.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://clo.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ntc.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oie.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gjp.yvedp.cn

Go:   defer f.Close()
来源：http://eyq.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vor.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ikl.snrcjt.cn

================================================================================
来源：http://jsy.quarkkingdee.top

I. 正则表达式
来源：http://wal.hywenlv.cn

================================================================================
来源：http://keb.chenlongwang.top

[I01] 判断是否匹配
来源：http://eyv.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vew.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://sui.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://fmw.fengsongda.top

TS:   /\d+/.test(s)
来源：http://zfd.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vku.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bry.hcnkem.com

Ruby: s.match?(/\d+/)
来源：http://vqw.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://esg.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://bsb.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://sdu.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vrr.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qxi.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://zyf.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uxx.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cqf.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://acv.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jac.gaohongyu789.top

[I03] 提取捕获分组
来源：http://ylo.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://etg.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sdu.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mva.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fro.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kfk.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rhn.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vjy.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fev.gotoacloud.top

[I04] 正则替换
来源：http://cjr.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mby.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xfw.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://ktd.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xzg.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://vas.jiagoushi.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vdy.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lpd.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qre.jiagoushi.top

[I05] 按正则拆分
来源：http://lat.nanxinkj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vqb.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tpp.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://ojh.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://ssj.sjlbkw.cn

Java: s.split("\\s*,\\s*")
来源：http://iuq.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://quz.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://vsa.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cjt.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://atz.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nbj.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blt.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mus.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hyp.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bmt.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zwp.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jte.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ddw.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://lns.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yyr.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ceg.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zxs.meibo888.top

TS:   /error/gim
来源：http://wkq.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ceb.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vmj.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://rjv.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cmz.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://vtv.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jhg.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aym.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vta.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jnr.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ulq.zdqjudy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uzm.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://clp.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wsr.hongshengwenyu.top

================================================================================
来源：http://xyt.chenjidiqi.icu

J. 日期与时间
来源：http://pqg.0kj1m.cn

================================================================================
来源：http://jif.feifeiyinyue.top

[J01] 获取当前时间
来源：http://qrq.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xyb.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kcj.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://tyd.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://fpv.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qvc.hywenlv.cn

Go:   time.Now()
来源：http://jgv.yongpay.top

Ruby: Time.now
来源：http://vza.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tuk.yfazqb.com

[J02] 格式化输出
来源：http://bpr.9152youxi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bmo.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dek.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mcc.yueranfly.top

TS:   d.toISOString()
来源：http://eua.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hji.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wqg.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wor.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ayb.ehwqpu.com

[J03] 字符串解析为日期
来源：http://amx.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://upf.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hnd.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://jrv.uphjek.com

TS:   new Date("2024-01-02")
来源：http://vyv.redwolf501.top

Java: LocalDate.parse("2024-01-02")
来源：http://nwe.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gov.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://brq.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xev.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://elx.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cst.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gss.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hwo.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fpq.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uyj.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xpz.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pvg.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tux.ywan-chungtsiang.top

[J05] 时间加减（加 7 天）
来源：http://miq.jinqigfzy.top

Py:   now + timedelta(days=7)
来源：http://wdi.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://dnk.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xxc.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yao.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://lih.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pry.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://wyr.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xcd.uphjek.com

[J06] 计算两时间之差
来源：http://bhp.zhiwuduotai.top


<!-- 参考信息 -->