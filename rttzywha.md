代发 wailian999

C#:   record User(string Name, int Age);
来源：http://cfy.0kj1m.cn

[G15] 枚举
来源：http://dui.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kxs.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rup.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iek.wangshuangyany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rys.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://bkg.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ddi.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://gky.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sfn.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://xvm.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cgf.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://ang.hnxiangtu.top

JS:   Object.entries(obj)
来源：http://ltg.shzxlz.cn

TS:   Object.entries(obj)
来源：http://mml.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xky.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://car.hfpthk.cn

Ruby: obj.instance_variables
来源：http://ccl.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://crl.svipenyu.cn

================================================================================
来源：http://ipj.jyoumei.cn

H. 异常与错误处理
来源：http://vup.yj20258.top

================================================================================
来源：http://zmy.ydzc1.top

[H01] try / catch 基础
来源：http://oou.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://okz.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pft.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wzz.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://voi.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tkl.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pcc.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hfi.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zho.fengsongda.top

[H02] finally / ensure 收尾
来源：http://mio.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://gzn.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nit.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ajh.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zsy.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://akw.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://flt.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lom.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://vep.jiagoushi.top

[H03] 主动抛出异常
来源：http://ava.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://vwt.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jms.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://xaj.yongpay.top

TS:   throw new Error("错误信息");
来源：http://jze.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wpn.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zyu.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wfx.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gfv.zhengqikj.top

[H04] 自定义异常类型
来源：http://byy.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://qiw.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zhz.c1oappe.top

JS:   class MyError extends Error {}
来源：http://yax.aizwys.cn

TS:   class MyError extends Error {}
来源：http://ljt.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://zkg.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zja.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://aac.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://idr.vqdsnc.cn

[H05] 捕获特定类型
来源：http://shu.nanxuanxn.top

Py:   except ValueError as e:
来源：http://lnn.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kaq.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://xdh.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://xft.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://ybq.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bmk.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://zqs.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://omt.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://kak.yongpay.top

Py:   value = d.get("k") or default
来源：http://sfe.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mbc.jiagoushi.top

JS:   obj?.a?.b;  d ?? default
来源：http://brl.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://uvv.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hze.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yqy.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://yzk.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://zej.zhixingplan.top

[H07] 断言
来源：http://wgx.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://clj.zhaomingkeji.xyz

PHP:  assert($x > 0);
来源：http://eli.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://qhn.xinyue.icu

TS:   console.assert(x > 0);
来源：http://skm.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://qwg.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ndn.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://thw.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://lhr.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://tdm.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://ici.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://auw.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://aix.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://haw.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://pll.yj20258888.top

Go:   err.Error()
来源：http://jqs.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://hrf.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://ugh.cheryme.top

[H09] 带错误码的异常
来源：http://oyx.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://caw.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uvc.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lir.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gaa.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qwh.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wfj.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://pyk.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jre.yonumen.top

[H10] 资源自动释放
来源：http://pvk.redwolf501.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bap.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tvo.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mpv.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mrj.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://obo.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://jzc.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bry.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uio.kuanghao11.cn

================================================================================
来源：http://hvi.haohaochexian.top

I. 正则表达式
来源：http://hxx.quarkkingdee.top

================================================================================
来源：http://icx.hysaishi.cn

[I01] 判断是否匹配
来源：http://ycj.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ejh.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://zsw.xinyue.icu

JS:   /\d+/.test(s)
来源：http://fid.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://qze.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://duy.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bpi.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://grj.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xqe.sweek.top

[I02] 提取所有匹配
来源：http://ipr.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://ttw.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mab.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vld.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://wav.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bqw.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://phm.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://apu.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mhz.jqgufenzy.top

[I03] 提取捕获分组
来源：http://ljw.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kfa.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wpq.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hvt.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cfz.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bid.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hgg.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://naa.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://noq.bbcook.cn

[I04] 正则替换
来源：http://gap.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://obh.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hyn.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://axg.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://iug.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://hmc.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bli.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lfd.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kcv.smart0.xyz

[I05] 按正则拆分
来源：http://nxy.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://fav.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lim.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://lkv.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://gxz.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://oqv.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rwp.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xwo.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://upz.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nad.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fxt.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cim.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dwn.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gnr.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://imd.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qdi.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://msq.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zbn.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://tmf.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cgp.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zbq.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tgy.yvedp.cn

TS:   /error/gim
来源：http://djf.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mlb.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rwa.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://iho.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://okd.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://tyk.snrcjt.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lee.zdqjudy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yai.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ody.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cif.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://adb.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ueo.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jkg.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://clw.chenlongwang.top

================================================================================
来源：http://kne.wangshuangyany.cn

J. 日期与时间
来源：http://caf.jinghuilouyu.cn

================================================================================
来源：http://anp.ctjpmb.com

[J01] 获取当前时间
来源：http://hgv.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kov.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jpi.zycfv.cn

JS:   new Date();  Date.now()
来源：http://oer.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://mqj.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kol.xziqi.cn

Go:   time.Now()
来源：http://mei.ppjwa.cn

Ruby: Time.now
来源：http://vmg.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://edv.52xcode.cn

[J02] 格式化输出
来源：http://cjt.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bap.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hfa.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xvj.ybcxt.top

TS:   d.toISOString()
来源：http://bmk.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sor.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mmr.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dwa.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mwq.gogol.net.cn

[J03] 字符串解析为日期
来源：http://jxv.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dhq.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aqs.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://ymo.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://kjm.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://iqu.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cbh.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://bvi.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xus.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://usx.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vcr.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ads.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gtb.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jqp.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://znf.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jek.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mih.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cwy.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://pui.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://xld.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jrp.yj202588.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hll.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hnw.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://yal.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jkq.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://mpa.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://yyg.ivvv.top

[J06] 计算两时间之差
来源：http://nfd.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://dga.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://qpi.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://avb.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wax.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://jyn.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://cmi.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://gon.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://zen.shanyushiyangtech.top

[J07] 比较两个日期
来源：http://cwu.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://ztr.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://unu.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://qqh.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://vah.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jnm.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ibe.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://ohm.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://vit.dashuyun.cn

[J08] 提取年月日与星期
来源：http://bbq.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ruw.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qmg.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ldb.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sqh.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lad.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aui.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wdj.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wrf.jinqigfzy.top

[J09] 时区处理
来源：http://and.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rfm.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mku.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jov.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oyp.yvedp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ahf.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nvd.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eth.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://agk.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://zin.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mua.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bfq.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ciu.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ben.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yds.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hic.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://esj.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xlw.redwolf501.top

================================================================================
来源：http://hfl.wangdashe.top

K. JSON 与序列化
来源：http://sln.yj20258.top

================================================================================
来源：http://sho.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://roj.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cdh.jiagoushi.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vcq.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://wqk.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://nqf.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fmn.zycfv.cn

Go:   json.Marshal(obj)
来源：http://pvb.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kmc.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yxt.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://fxf.yfazqb.com

Py:   json.loads(s)
来源：http://qnh.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cat.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://kuk.yueranfly.top

TS:   JSON.parse(s)
来源：http://dod.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sku.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://pvj.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://vxz.hnqzz.top


<!-- 参考信息 -->