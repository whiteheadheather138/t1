代发 wailian999

PHP:  public static function f() {}
来源：http://laj.52xcode.cn

JS:   static f() {}
来源：http://gyr.ehwqpu.com

TS:   static f(): void {}
来源：http://xmb.jinyuanbaomall.cn

Java: static void f() {}
来源：http://vhv.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zpg.bjfxy.top

Ruby: def self.f; end
来源：http://nxi.hnxiangtu.top

C#:   public static void F() {}
来源：http://pwm.tanke756.top

[G09] 接口 / 抽象类
来源：http://kki.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://eom.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://jyl.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wvt.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://cjn.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://uyk.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://wnd.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ocj.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://mls.guowangkeji.top

[G10] 访问控制
来源：http://odr.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://umc.dashuyun.cn

PHP:  public / protected / private
来源：http://gey.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://mpv.jianghu66.top

TS:   public / protected / private
来源：http://yjs.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://bqh.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cpn.birdmap.top

Ruby: public / protected / private
来源：http://bid.nwbrower.top

C#:   public / protected / private / internal
来源：http://rww.zdbjq.cn

[G11] getter / setter
来源：http://zyu.ydzc1.top

Py:   @property 与 @x.setter
来源：http://wbe.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ziz.yj202588.top

JS:   get name() { return this._name; }
来源：http://kig.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://vqa.cdnleiting.top

Java: public String getName() { return name; }
来源：http://qgq.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://enh.tianlin.xyz

Ruby: attr_accessor :name
来源：http://qyz.xuanzx.com

C#:   public string Name { get; set; }
来源：http://yjv.tian-w.cn

[G12] 对象转字符串
来源：http://vsr.cheryme.top

Py:   def __str__(self): return self.name
来源：http://zpd.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ksn.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://eqv.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://jxj.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://pcb.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tlk.52xcode.cn

Ruby: def to_s; @name; end
来源：http://xvb.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://kgo.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://opo.yangfankeji.com

Py:   isinstance(u, User)
来源：http://hvr.yuanzhike.top

PHP:  $u instanceof User
来源：http://ubm.fzhhl.top

JS:   u instanceof User
来源：http://mfj.guowangkeji.top

TS:   u instanceof User
来源：http://kik.jianghu66.top

Java: u instanceof User
来源：http://bhb.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mfg.ydzc1.top

Ruby: u.is_a?(User)
来源：http://tto.kuanghao11.cn

C#:   u is User
来源：http://nzi.hywenlv.cn

[G14] 数据类 / record
来源：http://yfd.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xri.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://qyp.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://goj.nanxinkj.top

TS:   type User = { name: string; age: number };
来源：http://spe.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://ejb.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://osi.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bgr.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://upu.ydjk.org.cn

[G15] 枚举
来源：http://hud.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tpd.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ykv.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ypv.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yun.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://edj.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dkc.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://fxv.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qhu.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://uxg.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ktb.pycfn.com

PHP:  get_object_vars($obj);
来源：http://phv.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://dwm.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://wxq.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://brv.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qch.shzxlz.cn

Ruby: obj.instance_variables
来源：http://xcy.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://bjq.jlsjyb.cn

================================================================================
来源：http://muk.dianchejie.cn

H. 异常与错误处理
来源：http://fst.cheryme.top

================================================================================
来源：http://fwn.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://omo.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ipe.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dnw.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xrl.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://emo.hywenlv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vde.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://euq.guannengcc.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://srw.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://csx.jiagoushi.top

[H02] finally / ensure 收尾
来源：http://iqn.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://mpn.zhengqikj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hik.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tgs.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oai.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mha.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ccn.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://anx.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://oeu.xuanzx.com

[H03] 主动抛出异常
来源：http://ukp.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://jla.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bem.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://bpo.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://kya.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dkn.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mmz.tian-w.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cnq.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://nqk.zhixingplan.top

[H04] 自定义异常类型
来源：http://vax.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://avf.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://cfz.birdmap.top

JS:   class MyError extends Error {}
来源：http://lcy.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://ctb.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://hbi.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ryu.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://bfe.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://zis.zdbjq.cn

[H05] 捕获特定类型
来源：http://dcm.fktsv.cn

Py:   except ValueError as e:
来源：http://ezy.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ske.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://pzx.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://men.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://xwf.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://swu.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://bnl.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sgj.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://pvd.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://hfh.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://vsi.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://zlx.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://zag.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rei.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hze.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://pxr.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://ijc.hfpthk.cn

[H07] 断言
来源：http://yiq.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://fld.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://eyk.mhx1999.top

JS:   console.assert(x > 0);
来源：http://kkd.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://evr.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://tme.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://woe.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://qes.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://qls.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://cpr.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://fjs.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kgz.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://ztp.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qlr.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dyk.jinyuanbaomall.cn

Go:   err.Error()
来源：http://rlf.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://qhk.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://wmm.hnqzz.top

[H09] 带错误码的异常
来源：http://zzp.jinyuanbaomall.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jew.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://lhv.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qww.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qdk.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wqb.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vde.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qci.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gfe.cheryme.top

[H10] 资源自动释放
来源：http://gju.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqu.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rlx.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tqf.hnqzz.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eyg.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cay.zhongyouzk.top

Go:   defer f.Close()
来源：http://ttf.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lvx.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://axs.jqgfzy.top

================================================================================
来源：http://ted.cucudq.cn

I. 正则表达式
来源：http://yhd.hfpthk.cn

================================================================================
来源：http://fjc.yuxming.cn

[I01] 判断是否匹配
来源：http://iiy.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ixw.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://wic.316326.xyz

JS:   /\d+/.test(s)
来源：http://bcc.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://alx.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hks.tarul.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zwm.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://gry.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vuc.52xcode.cn

[I02] 提取所有匹配
来源：http://xwe.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://ppd.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qmv.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pva.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://ivm.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cyy.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bbz.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://ymq.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pzj.vehdjk.com

[I03] 提取捕获分组
来源：http://ped.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ofz.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gvr.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://abi.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eeg.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jbd.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://amd.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ssb.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hmg.yj202588.top

[I04] 正则替换
来源：http://mqk.52xcode.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gnc.jqgfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hmx.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://zsp.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://pmf.jiagoushi.top

Java: s.replaceAll("\\d+", "#")
来源：http://gyf.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aba.jyoumei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gqt.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hxb.mhx1999.top

[I05] 按正则拆分
来源：http://njq.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cct.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mkg.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://kvf.zdqjudy.top

TS:   s.split(/\s*,\s*/)
来源：http://gcf.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://zoj.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://usv.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://ecy.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nfa.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lvf.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tga.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zqg.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yvi.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hyt.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dvd.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ppr.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bsm.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nii.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://efd.xylfe.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kvb.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hyi.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uma.mhx1999.top

TS:   /error/gim
来源：http://byo.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://muu.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nrj.yfazqb.com

Ruby: s.scan(/error/i)
来源：http://spy.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://svf.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://inu.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rbs.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mtc.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmz.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nir.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bcg.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hfg.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bpj.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pir.cucudq.cn

================================================================================
来源：http://wse.ydjk.org.cn

J. 日期与时间
来源：http://ulw.redwolf501.top

================================================================================
来源：http://rrb.zhongyouzk.top

[J01] 获取当前时间
来源：http://ttt.zhongyouzk.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://gmy.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pvz.cashguo.top

JS:   new Date();  Date.now()
来源：http://ftt.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://cwu.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://czc.andypj.xyz

Go:   time.Now()
来源：http://gop.fengsongda.top

Ruby: Time.now
来源：http://fko.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kof.chenzaomai.com

[J02] 格式化输出
来源：http://pit.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pji.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gkz.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uxa.tianlin.xyz

TS:   d.toISOString()
来源：http://dro.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xrt.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mcs.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://acu.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pls.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://nce.fehbvm.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://biq.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://luv.cashguo.top

JS:   new Date("2024-01-02")
来源：http://aek.gotoacloud.top

TS:   new Date("2024-01-02")
来源：http://ieb.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dek.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hxj.fengsongda.top

Ruby: Date.parse("2024-01-02")
来源：http://wup.sysykeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hrm.guannengcc.top

[J04] 时间戳与日期互转
来源：http://nmt.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jwd.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wrv.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vnv.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://fwo.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qhc.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ldi.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lpw.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oik.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://jwu.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://drg.feifeiyinyue.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://djc.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aiw.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://arz.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://ntq.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uah.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://xzm.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://xxs.redwolf501.top

[J06] 计算两时间之差
来源：http://mmv.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://ibq.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://cex.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qgb.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wfz.daxiang520.top


<!-- 参考信息 -->