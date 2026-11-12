代发 wailian999

Java: u instanceof User
来源：http://xhz.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jke.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://nrh.pengpengdd.cyou

C#:   u is User
来源：http://uag.guannengcc.top

[G14] 数据类 / record
来源：http://dbm.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qbq.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://yim.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://tvq.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://qca.316326.xyz

Java: record User(String name, int age) {}
来源：http://hno.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://shv.svipenyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cii.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://zty.52xcode.cn

[G15] 枚举
来源：http://vft.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hlm.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://akn.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bxu.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wog.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://qwx.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zys.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://soq.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kxt.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://hbq.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aqi.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://srw.ctjpmb.com

JS:   Object.entries(obj)
来源：http://rol.guowangkeji.top

TS:   Object.entries(obj)
来源：http://fct.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://veg.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://slk.yfazqb.com

Ruby: obj.instance_variables
来源：http://ges.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://pkg.quarkkingdee.top

================================================================================
来源：http://jfp.hnxiangtu.top

H. 异常与错误处理
来源：http://ycf.fehbvm.com

================================================================================
来源：http://kij.c1oappe.top

[H01] try / catch 基础
来源：http://okb.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ngw.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zzs.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pif.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eaf.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ypc.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ity.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vzn.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zzt.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://bid.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wrt.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wbr.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ccu.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lvv.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://whm.shzxlz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://euf.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bsz.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nyv.xuanzx.com

[H03] 主动抛出异常
来源：http://lmb.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://tjs.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eso.bjfxy.top

JS:   throw new Error("错误信息");
来源：http://wzp.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://oqr.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fgn.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cvp.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://egm.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://rkk.hesvh.cn

[H04] 自定义异常类型
来源：http://kof.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://rvz.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uuz.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://lyj.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://biy.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://gno.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wet.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://kvi.hcnkem.com

C#:   class MyException : Exception {}
来源：http://dtv.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://cbi.zhixingplan.top

Py:   except ValueError as e:
来源：http://gby.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qrr.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://qpf.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://jvr.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://pmo.zhixingplan.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fyn.chenzaomai.com

Ruby: rescue ArgumentError => e
来源：http://brf.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fxn.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://oax.xuanzx.com

Py:   value = d.get("k") or default
来源：http://ydx.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://chu.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://iww.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gvf.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zxt.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cbd.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://txm.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://adp.xuetiantiany.cn

[H07] 断言
来源：http://oxx.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://tys.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://lvm.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://mzk.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://kkw.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://oeo.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zfm.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ivt.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://asa.sweek.top

[H08] 获取错误信息与堆栈
来源：http://col.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://puj.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mgm.hnqzz.top

JS:   e.message;  e.stack
来源：http://kqk.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://wsp.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tyz.sxryk.cn

Go:   err.Error()
来源：http://aaz.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://inc.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://syk.zhengqikj.top

[H09] 带错误码的异常
来源：http://lzb.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kde.jianghu66.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rno.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qgk.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cnw.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jhs.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yfe.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://pji.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://jtv.yj20258.top

[H10] 资源自动释放
来源：http://hop.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://kmb.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://haq.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kid.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jgz.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lvn.redwolf501.top

Go:   defer f.Close()
来源：http://ttt.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ctv.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://koh.dashuyun.cn

================================================================================
来源：http://oyg.chenlongwang.top

I. 正则表达式
来源：http://fyl.nanxinkj.top

================================================================================
来源：http://mwc.sufxvd.cn

[I01] 判断是否匹配
来源：http://nix.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hxl.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pit.jianghu66.top

JS:   /\d+/.test(s)
来源：http://jtj.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://czv.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yhg.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zfg.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://emg.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ntp.guowangkeji.top

[I02] 提取所有匹配
来源：http://bwn.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://fai.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ogf.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uhn.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://ayj.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dby.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kig.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://ilc.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://quj.guowangkeji.top

[I03] 提取捕获分组
来源：http://zha.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://btj.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xqo.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dts.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tky.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xrh.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fez.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hna.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uqp.yonumen.top

[I04] 正则替换
来源：http://fkx.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xqd.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pti.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hmh.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://clb.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://fir.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nwr.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kzj.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lma.hcnkem.com

[I05] 按正则拆分
来源：http://mxv.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://crz.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ndy.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://nbn.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://vbd.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://xrw.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://snj.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://txe.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wxy.c1oappe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cqt.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ozj.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tsm.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://adr.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bgm.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ggc.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xqg.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pcz.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jxz.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://jmt.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jtt.fktsv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ovt.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://too.jinyuanbaomall.cn

TS:   /error/gim
来源：http://fug.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ech.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zcx.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://vdl.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kmc.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://vxj.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yyt.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://asp.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iag.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rvw.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ueu.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ixz.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://foe.jiagoushi.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yyo.jyoumei.cn

================================================================================
来源：http://qnq.jinqigfzy.top

J. 日期与时间
来源：http://dfh.ehwqpu.com

================================================================================
来源：http://xsp.cheryme.top

[J01] 获取当前时间
来源：http://tqv.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jud.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://alt.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://dgx.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://gdn.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vmy.zhoulong.xyz

Go:   time.Now()
来源：http://ddy.wangdashe.top

Ruby: Time.now
来源：http://wau.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://prm.yj20258888.top

[J02] 格式化输出
来源：http://pqx.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ske.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jqv.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bax.jlsjyb.cn

TS:   d.toISOString()
来源：http://aai.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cih.gotoacloud.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zzv.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yga.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bkm.birdmap.top

[J03] 字符串解析为日期
来源：http://der.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xai.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kqz.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://gac.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://svl.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://elh.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iyu.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://qnm.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aue.xinyue.icu

[J04] 时间戳与日期互转
来源：http://cte.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cjw.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dgs.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jjc.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://tvi.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nwd.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aht.fzhhl.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zfj.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ksi.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://ycs.yj20258.top

Py:   now + timedelta(days=7)
来源：http://hph.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vkh.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yvr.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fdc.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://oqs.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zeu.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://psc.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mfq.cashguo.top

[J06] 计算两时间之差
来源：http://vty.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://jyj.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://czo.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pat.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fms.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://rem.bjfxy.top

Go:   end.Sub(start).Hours()
来源：http://par.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://zer.ppjwa.cn

C#:   (end - start).TotalSeconds
来源：http://iyb.chenzaomai.com

[J07] 比较两个日期
来源：http://bpr.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://dlo.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pzp.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iwe.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://xzs.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uok.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ygo.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mlj.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://zkz.ehwqpu.com

[J08] 提取年月日与星期
来源：http://cti.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ilz.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mwg.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://amm.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ioe.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lxt.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://orl.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ioa.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fye.xuetiantiany.cn

[J09] 时区处理
来源：http://qkf.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wab.fanxiaobao.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yvx.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ofu.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ibp.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kpw.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ihz.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pop.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mpb.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://bag.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kwk.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bvg.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ifi.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zkz.316326.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fna.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://imi.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xtm.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xxh.yvedp.cn

================================================================================
来源：http://huz.vqdsnc.cn

K. JSON 与序列化
来源：http://zxg.quarkkingdee.top

================================================================================
来源：http://reb.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://jee.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://its.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xve.havefunace.top

JS:   JSON.stringify(obj)
来源：http://spc.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://sdf.chenlongwang.top


<!-- 参考信息 -->