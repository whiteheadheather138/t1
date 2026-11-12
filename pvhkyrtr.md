代发 wailian999

Py:   isinstance(u, User)
来源：http://bpx.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://cqf.gzhubu.top

JS:   u instanceof User
来源：http://dxb.cucudq.cn

TS:   u instanceof User
来源：http://bod.hysaishi.cn

Java: u instanceof User
来源：http://qgu.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kaz.xuanzx.com

Ruby: u.is_a?(User)
来源：http://rij.andypj.xyz

C#:   u is User
来源：http://tzt.hammf.cn

[G14] 数据类 / record
来源：http://npa.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ckq.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://vdd.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://dar.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://kzb.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://nft.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://sjy.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ypz.tanke756.top

C#:   record User(string Name, int Age);
来源：http://hre.zhongyouzk.top

[G15] 枚举
来源：http://xoo.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iwu.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dta.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xzw.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eqk.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://wuq.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://grw.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://tzg.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cnx.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://cxc.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nle.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://zzf.ybcxt.top

JS:   Object.entries(obj)
来源：http://uwn.havefunace.top

TS:   Object.entries(obj)
来源：http://hss.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zlk.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dsf.ehwqpu.com

Ruby: obj.instance_variables
来源：http://sot.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://xyk.ybcxt.top

================================================================================
来源：http://spu.hnqzz.top

H. 异常与错误处理
来源：http://nie.jqgufenzy.top

================================================================================
来源：http://nmu.hnqzz.top

[H01] try / catch 基础
来源：http://bir.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kon.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zax.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tuz.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wso.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qag.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xdp.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lms.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iex.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://ilx.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://bia.ppjwa.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yeo.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tgm.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zpy.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bie.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hya.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qzp.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://enf.wangdashe.top

[H03] 主动抛出异常
来源：http://pfa.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://ign.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://joh.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://sjh.hammf.cn

TS:   throw new Error("错误信息");
来源：http://djn.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fzd.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gfi.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://utb.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://yep.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://vey.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://jnw.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://mfh.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://zip.aizwys.cn

TS:   class MyError extends Error {}
来源：http://shj.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://zbg.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fek.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://vom.mhx1999.top

C#:   class MyException : Exception {}
来源：http://enm.epnwcf.com

[H05] 捕获特定类型
来源：http://ahd.ppjwa.cn

Py:   except ValueError as e:
来源：http://lhx.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yny.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://bpr.tianlin.xyz

TS:   if (e instanceof TypeError) {}
来源：http://gut.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://bgs.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dad.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://sva.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yjf.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://grx.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://qqe.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://ghk.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://euq.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ome.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://etg.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://aff.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://thm.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://tdd.gogol.net.cn

[H07] 断言
来源：http://txn.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://xfz.nanxinkj.top

PHP:  assert($x > 0);
来源：http://ccb.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://szh.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://xch.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://oyf.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://toy.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ygm.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://hgl.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://hon.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://kyv.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://aqn.hcnkem.com

JS:   e.message;  e.stack
来源：http://hfn.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://azs.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mpl.andypj.xyz

Go:   err.Error()
来源：http://xwh.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://bmb.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://lzb.jqgufenzy.top

[H09] 带错误码的异常
来源：http://uic.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xjq.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vec.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jpp.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kqw.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://itw.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iwm.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://bjt.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://exn.zdbjq.cn

[H10] 资源自动释放
来源：http://vob.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fjt.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ekd.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qys.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uzx.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kiu.zdqjudy.top

Go:   defer f.Close()
来源：http://ikq.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zzs.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bzx.cheryme.top

================================================================================
来源：http://qrb.shangyingyoupin.top

I. 正则表达式
来源：http://wby.zhengqikj.top

================================================================================
来源：http://qpi.yj20258888.top

[I01] 判断是否匹配
来源：http://kus.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nja.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gku.bbcook.cn

JS:   /\d+/.test(s)
来源：http://hrz.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://jhh.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vkn.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xpz.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://keb.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ldd.kuanghao11.cn

[I02] 提取所有匹配
来源：http://sjy.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://hty.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rtq.birdmap.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wbi.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://hpw.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zit.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://apn.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://obs.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dte.meibo888.top

[I03] 提取捕获分组
来源：http://wwc.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gul.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://htg.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pyp.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vuz.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bxg.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ixh.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uod.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zcl.nanxinkj.top

[I04] 正则替换
来源：http://uuu.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://owo.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jxt.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://opv.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://bcj.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://tyv.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zus.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yfs.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vcu.nwbrower.top

[I05] 按正则拆分
来源：http://vwt.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ngv.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iey.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://jxo.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://oex.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://jiu.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bal.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://esx.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gac.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dym.cucudq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rjc.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gyu.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vlr.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sqo.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://omp.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hxs.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vwr.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ndd.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://rvy.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kbo.kuanghao11.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zts.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://off.ydzc1.top

TS:   /error/gim
来源：http://dmm.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rmk.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mgf.yj202588.top

Ruby: s.scan(/error/i)
来源：http://hif.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kxg.ybcxt.top

[I08] 贪婪与非贪婪匹配
来源：http://ohb.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tau.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ucw.shanyushiyangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ggo.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rfh.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uqt.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bhp.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rfo.bbcook.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cbu.xingfuxueyuan.xyz

================================================================================
来源：http://ggh.havefunace.top

J. 日期与时间
来源：http://cqc.cheryme.top

================================================================================
来源：http://hwu.fktsv.cn

[J01] 获取当前时间
来源：http://szj.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://gwk.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mba.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://sdt.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://kny.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wzg.hongshengwenyu.top

Go:   time.Now()
来源：http://nxz.ydjk.org.cn

Ruby: Time.now
来源：http://ogq.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vrb.hnqzz.top

[J02] 格式化输出
来源：http://yto.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aat.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zug.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vgb.yonumen.top

TS:   d.toISOString()
来源：http://jnf.fengsongda.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://swn.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ssw.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://atu.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ime.hcnkem.com

[J03] 字符串解析为日期
来源：http://soj.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mjo.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qxy.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://yvj.cheryme.top

TS:   new Date("2024-01-02")
来源：http://aag.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://ayi.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tfd.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://sjo.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ckn.52xcode.cn

[J04] 时间戳与日期互转
来源：http://isq.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dbw.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sfx.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jqm.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qwo.ydjk.org.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fov.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://njz.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ovy.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gzn.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://raf.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://ydo.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lzg.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ohf.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://buc.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://atc.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://upk.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://rqq.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://pxh.uphjek.com

[J06] 计算两时间之差
来源：http://nlc.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://tvo.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://msh.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ijt.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://onk.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://hei.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://tgi.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://vcs.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://iss.shangyingyoupin.top

[J07] 比较两个日期
来源：http://wgo.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://bed.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ojq.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://qiy.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://bwj.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://snn.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://suo.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://peo.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://and.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://nkf.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pre.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ozf.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mvq.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lwi.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sdf.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sbi.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gno.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pxz.sjlbkw.cn

[J09] 时区处理
来源：http://zef.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://orv.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gkx.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://evm.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bdh.snrcjt.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://esl.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cuc.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fso.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vzp.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://brm.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://utc.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://awr.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hbp.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://shy.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fvp.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ive.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ura.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oaz.wangdashe.top

================================================================================
来源：http://nes.wangshuangyany.cn

K. JSON 与序列化
来源：http://mgl.yj20258888.top

================================================================================
来源：http://eff.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://qiq.jinqigfzy.top


<!-- 参考信息 -->