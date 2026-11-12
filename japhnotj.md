代发 wailian999

Java: interface Shape { double area(); }
来源：http://wzj.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://dah.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gii.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://gfb.shanyushiyangkeji.top

[G10] 访问控制
来源：http://lil.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://mpp.jinqigufen.top

PHP:  public / protected / private
来源：http://zjb.yj202588.top

JS:   #private 字段；其余公开
来源：http://bzb.yongpay.top

TS:   public / protected / private
来源：http://tpr.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://gko.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://qky.shangyingyoupin.top

Ruby: public / protected / private
来源：http://xwq.yj202588.top

C#:   public / protected / private / internal
来源：http://wnk.tian-w.cn

[G11] getter / setter
来源：http://ujc.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://njb.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://abl.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://ehx.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://csx.316326.xyz

Java: public String getName() { return name; }
来源：http://iiz.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://yqh.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://nyp.fengsongda.top

C#:   public string Name { get; set; }
来源：http://rfj.jianghu66.top

[G12] 对象转字符串
来源：http://sqp.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://abp.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sxa.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://xkc.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://jnr.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://isp.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iit.vehdjk.com

Ruby: def to_s; @name; end
来源：http://vpr.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://gns.yj202588.top

[G13] 判断对象类型
来源：http://lpf.tarul.cn

Py:   isinstance(u, User)
来源：http://vuo.smart0.xyz

PHP:  $u instanceof User
来源：http://nft.snrcjt.cn

JS:   u instanceof User
来源：http://iub.tarul.cn

TS:   u instanceof User
来源：http://ymw.zhoulong.xyz

Java: u instanceof User
来源：http://xgr.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://min.52xcode.cn

Ruby: u.is_a?(User)
来源：http://wgz.c1oappe.top

C#:   u is User
来源：http://ubk.daria6918.cn

[G14] 数据类 / record
来源：http://llj.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qzs.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://ogk.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xlz.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://syh.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://rzs.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://nus.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mhh.yj20258.top

C#:   record User(string Name, int Age);
来源：http://wox.yuanzhike.top

[G15] 枚举
来源：http://bpz.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ykt.uphjek.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://kbf.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qhm.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qif.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://ljt.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lqy.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://flf.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mvq.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://jnk.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zid.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://gqf.ctjpmb.com

JS:   Object.entries(obj)
来源：http://twp.chenzaomai.com

TS:   Object.entries(obj)
来源：http://umy.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rcx.shangyingyoupin.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ita.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://vkl.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://fvh.wangshuangyany.cn

================================================================================
来源：http://vch.ydjk.org.cn

H. 异常与错误处理
来源：http://axl.sjlbkw.cn

================================================================================
来源：http://zhn.hongshengwenyu.top

[H01] try / catch 基础
来源：http://yfi.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://myu.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ciq.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gga.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fqq.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uap.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nar.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zyv.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ycg.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://loz.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://cut.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rhm.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mmk.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://brt.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://grz.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cym.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pms.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dkf.daria6918.cn

[H03] 主动抛出异常
来源：http://szc.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://tau.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oax.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://akf.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://scz.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://asx.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kti.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ofv.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://dkv.wangdashe.top

[H04] 自定义异常类型
来源：http://xcj.birdmap.top

Py:   class MyError(Exception): pass
来源：http://xqb.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bjd.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://buu.guannengcc.top

TS:   class MyError extends Error {}
来源：http://ach.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://lju.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zcm.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://vja.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://efn.xuanzx.com

[H05] 捕获特定类型
来源：http://atq.xinyue.icu

Py:   except ValueError as e:
来源：http://jqj.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ixf.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://oxn.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://uqs.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://tok.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zac.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://fti.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ali.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://rtw.ivvv.top

Py:   value = d.get("k") or default
来源：http://jms.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uex.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://rcb.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://abh.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pfa.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ygj.xuetiantiany.cn

Ruby: d&.dig(:a, :b)
来源：http://afy.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://sgc.jqgfzy.top

[H07] 断言
来源：http://lvk.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://bum.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://wrv.epnwcf.com

JS:   console.assert(x > 0);
来源：http://onb.pycfn.com

TS:   console.assert(x > 0);
来源：http://zpz.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://liy.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uuf.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://ply.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://zlx.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://pnt.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://cfn.zdbjq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ivi.zycfv.cn

JS:   e.message;  e.stack
来源：http://fyi.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pqj.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cff.shanyushiyangtech.top

Go:   err.Error()
来源：http://feh.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://jfl.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://wfc.zdqjudy.top

[H09] 带错误码的异常
来源：http://mpl.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dkj.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nnu.hysaishi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ceb.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://umm.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lxz.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://azl.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jim.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://flq.uphjek.com

[H10] 资源自动释放
来源：http://rjo.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xyx.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://psu.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mqx.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jmi.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hlu.vehdjk.com

Go:   defer f.Close()
来源：http://aic.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cjk.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wld.guowangkeji.top

================================================================================
来源：http://qjj.smart0.xyz

I. 正则表达式
来源：http://fyt.xinyue.icu

================================================================================
来源：http://pui.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://kfz.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://axe.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://jfa.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://tnp.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://eft.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xvj.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bzo.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://iax.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dxh.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://ead.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://bml.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qyg.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mqm.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://gce.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bbl.guannengcc.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aml.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://uft.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jfc.zdbjq.cn

[I03] 提取捕获分组
来源：http://ubu.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://whm.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ohq.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oeu.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fds.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hud.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kes.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mqf.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qol.yanxiufei.cn

[I04] 正则替换
来源：http://ztz.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tcp.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dnb.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://koy.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xdr.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://gbq.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vgk.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qrz.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ram.meibo888.top

[I05] 按正则拆分
来源：http://cnk.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uur.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xqf.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://hcu.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://quq.bbcook.cn

Java: s.split("\\s*,\\s*")
来源：http://htf.zdbjq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gkn.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mqe.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bwl.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yxs.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sbt.zdqjudy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ngf.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lau.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qht.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zmn.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zyx.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uss.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zid.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://wtg.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fhd.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nhx.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aml.guowangkeji.top

TS:   /error/gim
来源：http://dhi.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ujy.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oif.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://swq.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pyt.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://vpr.nanxinkj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hfb.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bcv.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xzy.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rqm.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://dbx.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://alz.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tnn.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://njx.tian-w.cn

================================================================================
来源：http://ykp.ivvv.top

J. 日期与时间
来源：http://xba.aibaodan.cn

================================================================================
来源：http://jzs.hywenlv.cn

[J01] 获取当前时间
来源：http://mnx.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://lix.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wqc.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://phz.gzhubu.top

TS:   new Date();  Date.now()
来源：http://wkn.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kpp.hnqzz.top

Go:   time.Now()
来源：http://nxx.hongshengwenyu.top

Ruby: Time.now
来源：http://qfn.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ybk.gzhubu.top

[J02] 格式化输出
来源：http://qrj.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aiu.zdqjudy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vwk.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nwk.fehbvm.com

TS:   d.toISOString()
来源：http://pxj.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vwy.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kqr.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oca.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rwr.svipenyu.cn

[J03] 字符串解析为日期
来源：http://ddo.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nic.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gal.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://ids.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://hvz.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://sfu.yvedp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kdi.yanxiufei.cn

Ruby: Date.parse("2024-01-02")
来源：http://kmc.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bin.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://uoo.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://imd.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://szg.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ejv.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rhy.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://btr.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pwj.svipenyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kdu.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gap.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://kek.feifeiyinyue.top

Py:   now + timedelta(days=7)
来源：http://vlo.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://smh.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ftm.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fcq.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://lei.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fog.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://sjq.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vuv.smart0.xyz

[J06] 计算两时间之差
来源：http://fkq.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://gme.wangdashe.top

PHP:  $end->diff($start)->days;
来源：http://ifs.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://scj.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zko.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://sdw.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://seu.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://suz.yj202588.top

C#:   (end - start).TotalSeconds
来源：http://qtr.hesvh.cn

[J07] 比较两个日期
来源：http://jny.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://ifg.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zfj.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://bzh.hfpthk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yyx.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://odf.ybcxt.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://unl.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://swg.hywenlv.cn


<!-- 参考信息 -->