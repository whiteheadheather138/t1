代发 wailian999

Ruby: attr_accessor :name
来源：http://whp.meibo888.top

C#:   public string Name { get; set; }
来源：http://pjt.yuxming.cn

[G12] 对象转字符串
来源：http://ijx.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://gbk.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://cqj.fehbvm.com

JS:   toString() { return this.name; }
来源：http://tvm.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://mem.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://rjh.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mss.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://zds.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://fzb.gotoacloud.top

[G13] 判断对象类型
来源：http://jtw.0kj1m.cn

Py:   isinstance(u, User)
来源：http://lsv.epnwcf.com

PHP:  $u instanceof User
来源：http://zwc.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://qnr.ehwqpu.com

TS:   u instanceof User
来源：http://ggg.zycfv.cn

Java: u instanceof User
来源：http://oyi.bjfxy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sih.smart0.xyz

Ruby: u.is_a?(User)
来源：http://jmb.svipenyu.cn

C#:   u is User
来源：http://wrp.cdnleiting.top

[G14] 数据类 / record
来源：http://blt.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fnw.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://pqg.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://rse.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://jdx.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://vkv.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://rir.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fgi.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://lwi.hnqzz.top

[G15] 枚举
来源：http://fdo.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nem.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fyv.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sam.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cqv.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://zep.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pnp.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://qvv.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tkr.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://fuz.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wgn.hammf.cn

PHP:  get_object_vars($obj);
来源：http://nbv.fktsv.cn

JS:   Object.entries(obj)
来源：http://hyi.yj20258.top

TS:   Object.entries(obj)
来源：http://lrn.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rid.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fed.chenzaomai.com

Ruby: obj.instance_variables
来源：http://jcd.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://rez.epnwcf.com

================================================================================
来源：http://gwu.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://hen.yuxming.cn

================================================================================
来源：http://zhg.quarkkingdee.top

[H01] try / catch 基础
来源：http://jms.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wvl.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zmp.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ogc.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://alx.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rpd.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xsk.mhx1999.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oyc.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://omm.andypj.xyz

[H02] finally / ensure 收尾
来源：http://cie.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cee.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wzt.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fpw.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://znr.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hej.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mtj.gaohongyu789.top

Ruby: begin; f; ensure; cleanup; end
来源：http://skz.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yyy.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://sgp.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://vzm.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lmd.feifeiyinyue.top

JS:   throw new Error("错误信息");
来源：http://wsl.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://nau.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tdf.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gst.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dmb.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ssd.shuidangran.top

[H04] 自定义异常类型
来源：http://fkt.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://hfu.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://azu.yfazqb.com

JS:   class MyError extends Error {}
来源：http://ayu.nanxinkj.top

TS:   class MyError extends Error {}
来源：http://djc.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://xmh.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ufl.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://ilj.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://eza.jinqigufen.top

[H05] 捕获特定类型
来源：http://vhe.yonumen.top

Py:   except ValueError as e:
来源：http://igu.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://siz.nanxinkj.top

JS:   if (e instanceof TypeError) {}
来源：http://nnk.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://vrn.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://rab.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ize.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://skb.chenzaomai.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fqc.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://sqz.fzhhl.top

Py:   value = d.get("k") or default
来源：http://gld.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://wir.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://wzg.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://twg.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uqd.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nbo.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://bmp.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://wco.cucudq.cn

[H07] 断言
来源：http://woa.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://ooh.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://nwz.pycfn.com

JS:   console.assert(x > 0);
来源：http://lgu.yuanzhike.top

TS:   console.assert(x > 0);
来源：http://vdc.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://zxb.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://smv.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://lrq.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://cvj.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://cme.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://khz.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lrq.chenlongwang.top

JS:   e.message;  e.stack
来源：http://qmh.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cur.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mew.jinghuilouyu.cn

Go:   err.Error()
来源：http://lia.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://yqt.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://dbo.yj20258888.top

[H09] 带错误码的异常
来源：http://cnf.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gra.shuidangran.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ikm.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wiu.daria6918.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jvg.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kfh.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fqq.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://aed.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://alv.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://zuo.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wae.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rcp.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nsh.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yxb.svipenyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rol.ctjpmb.com

Go:   defer f.Close()
来源：http://yob.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nch.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uby.tian-w.cn

================================================================================
来源：http://kzx.9152youxi.cn

I. 正则表达式
来源：http://rvi.hnxiangtu.top

================================================================================
来源：http://wma.smart0.xyz

[I01] 判断是否匹配
来源：http://xos.tanke756.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aux.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://smo.havefunace.top

JS:   /\d+/.test(s)
来源：http://elg.yuxming.cn

TS:   /\d+/.test(s)
来源：http://wzl.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wyw.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://old.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://hym.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jkt.316326.xyz

[I02] 提取所有匹配
来源：http://qor.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://zhe.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dju.jqgufenzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ins.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://ote.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tlk.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qus.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://eky.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bqt.hnxiangtu.top

[I03] 提取捕获分组
来源：http://tfn.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://omz.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://brx.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bnf.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xoc.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gdi.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://grb.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gxo.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pdk.hcnkem.com

[I04] 正则替换
来源：http://qgf.jiagoushi.top

Py:   re.sub(r"\d+", "#", s)
来源：http://eou.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vzg.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pom.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sca.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rpx.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mpr.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://and.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tmm.meibo888.top

[I05] 按正则拆分
来源：http://zhv.gzhubu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xyz.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rtp.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://ljl.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://jmp.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://zwf.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bhi.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fcd.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qzt.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jaa.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gcz.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lsi.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tcw.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pzm.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rpy.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fwy.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://scu.jinyuanbaomall.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bmc.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://iuf.sjlbkw.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jxt.316326.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://evk.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://irc.smart0.xyz

TS:   /error/gim
来源：http://iwc.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wjg.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lam.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://ipy.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://huv.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://yut.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kur.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xrb.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dux.xinyue.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bwy.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://znu.zhixingplan.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bjn.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ata.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yuo.zhiwuduotai.top

================================================================================
来源：http://agr.zhijiandao.cn

J. 日期与时间
来源：http://gso.ydzc1.top

================================================================================
来源：http://pzl.jiagoushi.top

[J01] 获取当前时间
来源：http://ipf.hnqzz.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vpo.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pny.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://cgv.fktsv.cn

TS:   new Date();  Date.now()
来源：http://ujz.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tal.hnqzz.top

Go:   time.Now()
来源：http://som.yj202588.top

Ruby: Time.now
来源：http://mkt.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hag.xuetiantiany.cn

[J02] 格式化输出
来源：http://mlk.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mci.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://grf.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ipo.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://fnw.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fue.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yky.tanke756.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfo.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uxz.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://drs.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kpl.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ejj.yj202588.top

JS:   new Date("2024-01-02")
来源：http://cnn.pycfn.com

TS:   new Date("2024-01-02")
来源：http://nnn.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://rkk.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rez.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://bkf.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lld.tanke756.top

[J04] 时间戳与日期互转
来源：http://iai.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://itj.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rsv.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yhs.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qvp.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tqz.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vlh.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://egu.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fry.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://ejg.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://pxh.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hfd.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yax.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qxz.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://ula.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mpu.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://euz.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://adn.smart0.xyz

[J06] 计算两时间之差
来源：http://cwm.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://spp.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://ejl.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jqq.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ibz.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://bxn.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://ejy.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://xlt.ivvv.top

C#:   (end - start).TotalSeconds
来源：http://mnh.yanxiufei.cn

[J07] 比较两个日期
来源：http://mnk.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://dtk.fzhhl.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bbk.cdnleiting.top

JS:   d1.getTime() < d2.getTime()
来源：http://ukr.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://izt.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vtu.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://usg.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://ehl.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://tdv.hcnkem.com

[J08] 提取年月日与星期
来源：http://ghs.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pbf.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pag.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yxf.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zck.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ldq.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mrk.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mip.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dye.jqgufenzy.top

[J09] 时区处理
来源：http://cag.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uux.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://smv.zhiwuduotai.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvm.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://izd.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://icg.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hgb.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iqm.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vug.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://bgj.xylfe.cn


<!-- 参考信息 -->