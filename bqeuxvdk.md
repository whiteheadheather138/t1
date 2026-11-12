代发 wailian999

TS:   public / protected / private
来源：http://elo.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://xac.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qgp.redwolf501.top

Ruby: public / protected / private
来源：http://xsi.andypj.xyz

C#:   public / protected / private / internal
来源：http://nbd.jiagoushi.top

[G11] getter / setter
来源：http://ovj.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://jrh.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nmy.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://sxb.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://nmu.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://hts.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dst.nanxinkj.top

Ruby: attr_accessor :name
来源：http://pib.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://pqi.yueranfly.top

[G12] 对象转字符串
来源：http://pgl.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://wjt.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lln.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://sda.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://ikm.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://iry.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://xwz.52xcode.cn

Ruby: def to_s; @name; end
来源：http://xja.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://czm.hammf.cn

[G13] 判断对象类型
来源：http://xjg.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://tuj.vehdjk.com

PHP:  $u instanceof User
来源：http://mzl.sweek.top

JS:   u instanceof User
来源：http://txy.ywan-chungtsiang.top

TS:   u instanceof User
来源：http://xfn.jyoumei.cn

Java: u instanceof User
来源：http://jfw.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kxm.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://exn.9152youxi.cn

C#:   u is User
来源：http://ivq.xuetiantiany.cn

[G14] 数据类 / record
来源：http://elv.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jyt.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://mzo.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://txl.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://jph.feifeiyinyue.top

Java: record User(String name, int age) {}
来源：http://dxd.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://wwv.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qxn.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://kyi.cheryme.top

[G15] 枚举
来源：http://fnh.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://git.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://czu.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hpn.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fas.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://ire.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sfw.feifeiyinyue.top

Ruby: Color = %i[red green].freeze
来源：http://hnz.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ani.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://hac.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ylo.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://nen.svipenyu.cn

JS:   Object.entries(obj)
来源：http://lat.guannengcc.top

TS:   Object.entries(obj)
来源：http://eez.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ese.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bbb.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://vah.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://iew.shzxlz.cn

================================================================================
来源：http://hjf.cashguo.top

H. 异常与错误处理
来源：http://dku.shanyushiyangkeji.top

================================================================================
来源：http://ehj.tarul.cn

[H01] try / catch 基础
来源：http://tck.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lnp.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wqr.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bdh.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ofw.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fff.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uql.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rft.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sid.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://byn.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vsq.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://byl.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ujp.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aox.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://kem.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iel.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nix.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ilg.jyoumei.cn

[H03] 主动抛出异常
来源：http://hya.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://ydj.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ytc.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://cme.pycfn.com

TS:   throw new Error("错误信息");
来源：http://wee.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://wrn.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kyr.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vbn.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://kpx.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://ika.guowangkeji.top

Py:   class MyError(Exception): pass
来源：http://ghw.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ztr.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://mpg.fzhhl.top

TS:   class MyError extends Error {}
来源：http://oqf.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://agu.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yrk.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://eop.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://qgn.jqgufenzy.top

[H05] 捕获特定类型
来源：http://bhw.yj20258.top

Py:   except ValueError as e:
来源：http://qxp.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lch.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://jiy.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://msc.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://thr.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rfv.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://frv.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://igo.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://zkk.daria6918.cn

Py:   value = d.get("k") or default
来源：http://luv.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nnx.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://pwd.yanxiufei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zxt.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rnh.zhoulong.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://kez.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://rsy.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://ikn.tian-w.cn

[H07] 断言
来源：http://qjt.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://hqc.yongpay.top

PHP:  assert($x > 0);
来源：http://znl.tian-w.cn

JS:   console.assert(x > 0);
来源：http://tdx.shuidangran.top

TS:   console.assert(x > 0);
来源：http://ceg.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://lmj.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gzj.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://xvh.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://bof.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://ljv.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://nzr.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fxs.hammf.cn

JS:   e.message;  e.stack
来源：http://tzn.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ezp.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sno.yvedp.cn

Go:   err.Error()
来源：http://tag.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://tyf.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://vdp.hammf.cn

[H09] 带错误码的异常
来源：http://lyx.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kqx.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ztf.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dei.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kwf.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cny.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lcv.gzhubu.top

Ruby: raise MyError.new("fail", 500)
来源：http://skn.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ibx.guannengcc.top

[H10] 资源自动释放
来源：http://png.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zdc.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wnd.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://snx.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://foi.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xoo.ybcxt.top

Go:   defer f.Close()
来源：http://cex.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mxb.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pdp.aizwys.cn

================================================================================
来源：http://nzr.jlsjyb.cn

I. 正则表达式
来源：http://kvt.hesvh.cn

================================================================================
来源：http://hmm.gzhubu.top

[I01] 判断是否匹配
来源：http://lqj.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fzq.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wiz.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://xrw.hammf.cn

TS:   /\d+/.test(s)
来源：http://zpx.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ign.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vfq.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://pfi.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xll.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://fjh.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://ktx.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xuj.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iqa.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://tdd.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mhe.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cqn.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://vcr.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hgb.jianghu66.top

[I03] 提取捕获分组
来源：http://jkk.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bdq.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vbj.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qzb.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pbd.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hav.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kho.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nqm.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rhu.zdqjudy.top

[I04] 正则替换
来源：http://mns.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mqy.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fqo.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://imu.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://fsi.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tjm.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bmj.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vij.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pkh.xziqi.cn

[I05] 按正则拆分
来源：http://wra.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://twc.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zns.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://xzn.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://mlg.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://tlm.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gzo.ybcxt.top

Ruby: s.split(/\s*,\s*/)
来源：http://syb.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uco.havefunace.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zpq.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tqo.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://awh.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gox.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ytn.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mia.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rau.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mwd.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://owr.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://jlj.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rgp.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lnn.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jvv.cqqwz.cn

TS:   /error/gim
来源：http://vbu.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hsl.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ejs.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://wwb.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hak.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://nbn.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kgt.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vdx.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xop.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://idy.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ccy.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eao.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wud.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qnm.fanxiaobao.xyz

================================================================================
来源：http://edb.hnxiangtu.top

J. 日期与时间
来源：http://ixb.redwolf501.top

================================================================================
来源：http://tep.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://vsq.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://joe.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bhr.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://llc.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://usx.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kxf.hcnkem.com

Go:   time.Now()
来源：http://vvt.tarul.cn

Ruby: Time.now
来源：http://ejw.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tcu.feifeiyinyue.top

[J02] 格式化输出
来源：http://kre.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vgf.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vcq.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vxx.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://ecw.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xak.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dmm.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nzr.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pem.sxryk.cn

[J03] 字符串解析为日期
来源：http://bix.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ewk.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yrq.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://jzw.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://dgd.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jhn.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wgu.cdnleiting.top

Ruby: Date.parse("2024-01-02")
来源：http://gln.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nzk.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://kvc.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mpi.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rad.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oxj.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xvj.andypj.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://asn.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hck.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zzo.yueranfly.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ktl.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://zlz.redwolf501.top

Py:   now + timedelta(days=7)
来源：http://vct.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://njs.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ryt.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lpb.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://gzr.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kao.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://kcc.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://tdu.jiagoushi.top

[J06] 计算两时间之差
来源：http://cjl.pycfn.com

Py:   (end - start).total_seconds()
来源：http://pnd.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://brd.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uod.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://led.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://xtz.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://sim.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://deu.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://jkc.vehdjk.com

[J07] 比较两个日期
来源：http://vlc.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://wyg.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uix.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://doa.gotoacloud.top

TS:   d1.getTime() < d2.getTime()
来源：http://ssu.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wrc.yangfankeji.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wbn.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://zgv.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://owd.nanxinkj.top

[J08] 提取年月日与星期
来源：http://xbu.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rvl.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xfy.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://erq.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vad.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://laz.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kqi.pengpengdd.cyou


<!-- 参考信息 -->