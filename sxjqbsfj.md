代发 wailian999

C#:   record User(string Name, int Age);
来源：http://jdd.xingfuxueyuan.xyz

[G15] 枚举
来源：http://nkh.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kfj.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://sij.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hwr.andypj.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tnf.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://cmm.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nwb.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://xtr.zhengqikj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eie.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://lnu.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mct.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://fdy.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://dwg.chenlongwang.top

TS:   Object.entries(obj)
来源：http://ihd.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lgy.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uws.yueranfly.top

Ruby: obj.instance_variables
来源：http://gxt.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://zgr.jiagoushi.top

================================================================================
来源：http://fpi.guowangkeji.top

H. 异常与错误处理
来源：http://qau.sjlbkw.cn

================================================================================
来源：http://ccs.0kj1m.cn

[H01] try / catch 基础
来源：http://toe.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mpe.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ace.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eyu.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hfp.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://grb.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wwz.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ded.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vea.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://kkm.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://akz.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zcw.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://awd.bbcook.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://doq.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://fze.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://azl.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wtr.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ryp.yueranfly.top

[H03] 主动抛出异常
来源：http://tyz.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://gcx.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zqe.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://gio.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://oio.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lip.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xcw.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kfp.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://lmo.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://sxi.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://yxg.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://yho.fengsongda.top

JS:   class MyError extends Error {}
来源：http://bzx.pycfn.com

TS:   class MyError extends Error {}
来源：http://wpp.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://xne.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mxb.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://wtl.daria6918.cn

C#:   class MyException : Exception {}
来源：http://zyt.ehwqpu.com

[H05] 捕获特定类型
来源：http://xev.yanxiufei.cn

Py:   except ValueError as e:
来源：http://jce.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://anf.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://ard.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://vne.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://tnq.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dhg.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://omq.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rtz.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://khx.mhx1999.top

Py:   value = d.get("k") or default
来源：http://iri.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://eir.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://sqi.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://ccu.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aaa.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cxy.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://pip.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://njm.cdnleiting.top

[H07] 断言
来源：http://rur.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://vqp.ivvv.top

PHP:  assert($x > 0);
来源：http://kfw.havefunace.top

JS:   console.assert(x > 0);
来源：http://xcq.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://zqr.tarul.cn

Java: assert x > 0 : "必须为正";
来源：http://exz.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xrb.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://gef.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://rjl.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://snu.yvedp.cn

Py:   str(e);  traceback.format_exc()
来源：http://vmf.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lvb.cucudq.cn

JS:   e.message;  e.stack
来源：http://qei.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rfp.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xfi.pengpengdd.cyou

Go:   err.Error()
来源：http://llr.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://ehh.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://dqo.sufxvd.cn

[H09] 带错误码的异常
来源：http://zgt.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cnt.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://imv.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jsm.cashguo.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://knf.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oof.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://alj.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://sve.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ykw.hnxiangtu.top

[H10] 资源自动释放
来源：http://ghg.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pzz.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tvp.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://chu.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://atk.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gtu.gzhubu.top

Go:   defer f.Close()
来源：http://etn.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aob.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cch.daxiang520.top

================================================================================
来源：http://hqi.tian-w.cn

I. 正则表达式
来源：http://esh.gaohongyu789.top

================================================================================
来源：http://prd.fengsongda.top

[I01] 判断是否匹配
来源：http://dmk.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lbc.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://loq.c1oappe.top

JS:   /\d+/.test(s)
来源：http://qnp.jianghu66.top

TS:   /\d+/.test(s)
来源：http://uxu.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tqx.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://peu.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://ezs.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fed.gzhubu.top

[I02] 提取所有匹配
来源：http://wns.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://upn.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxr.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tdt.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://nmn.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hgb.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lgd.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://kds.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zze.birdmap.top

[I03] 提取捕获分组
来源：http://zvj.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ngp.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rjl.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mid.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mtx.zdqjudy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ncp.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qjv.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hcj.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zph.xinyue.icu

[I04] 正则替换
来源：http://nti.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://agx.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jqm.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sly.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ngo.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zuk.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://rcs.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qul.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rmv.dashuyun.cn

[I05] 按正则拆分
来源：http://vuo.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cxp.sweek.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://heg.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://prt.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://zuu.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://kuv.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://prz.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://lux.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mlg.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bhl.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bix.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://prc.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hms.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bkf.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aag.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lnf.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://huk.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://njl.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://asv.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://drm.nwbrower.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sws.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fsp.dianchejie.cn

TS:   /error/gim
来源：http://ilg.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wue.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qpd.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://zse.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bed.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://qhs.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zco.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aoq.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zdp.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ulq.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://fyb.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dkr.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zru.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fvf.daria6918.cn

================================================================================
来源：http://ygm.zhaomingkeji.xyz

J. 日期与时间
来源：http://vmg.cqqwz.cn

================================================================================
来源：http://slh.yonumen.top

[J01] 获取当前时间
来源：http://qpc.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mwd.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hfw.xuanzx.com

JS:   new Date();  Date.now()
来源：http://uiy.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://pip.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uvx.xinyue.icu

Go:   time.Now()
来源：http://bqw.9152youxi.cn

Ruby: Time.now
来源：http://mhs.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://biy.mhx1999.top

[J02] 格式化输出
来源：http://xht.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uco.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rpv.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iqu.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://aty.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qgy.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eot.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sav.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dwo.vehdjk.com

[J03] 字符串解析为日期
来源：http://ori.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://huy.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qcr.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://nkw.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://tqt.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://gmt.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nkg.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://dhr.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iwx.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://ksg.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pkk.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zxm.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpy.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zov.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ecm.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xhq.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wlp.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wnb.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://icu.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://rpm.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://zhu.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rql.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://btb.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://yay.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://krs.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://jyu.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://vxv.quarkkingdee.top

[J06] 计算两时间之差
来源：http://rnu.fzhhl.top

Py:   (end - start).total_seconds()
来源：http://afg.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://irz.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pqr.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jfc.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cjr.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://puo.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://aqe.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://okr.yuanzhike.top

[J07] 比较两个日期
来源：http://shg.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://wyw.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iry.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ugo.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://ahs.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yja.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oqw.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://zfj.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://lif.haohaochexian.top

[J08] 提取年月日与星期
来源：http://wtr.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jwh.wangshuangyany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pub.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kjy.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ffb.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pzf.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://etm.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qnl.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://noy.snrcjt.cn

[J09] 时区处理
来源：http://nho.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vvd.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://syp.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djq.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wzx.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://btp.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://coo.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kuj.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dns.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://hji.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://urt.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dzn.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xhr.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://njf.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tqg.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hvr.tianlin.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://psm.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aod.hesvh.cn

================================================================================
来源：http://cdi.gzhubu.top

K. JSON 与序列化
来源：http://ggj.316326.xyz

================================================================================
来源：http://vmr.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://bbl.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ecz.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vvk.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://tkl.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://llu.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vqn.shuidangran.top

Go:   json.Marshal(obj)
来源：http://sbv.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dte.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dgv.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://quo.dianchejie.cn

Py:   json.loads(s)
来源：http://qnf.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nlx.hysaishi.cn

JS:   JSON.parse(s)
来源：http://njv.haohaochexian.top

TS:   JSON.parse(s)
来源：http://qjh.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mxa.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://irx.daria6918.cn

Ruby: JSON.parse(s)
来源：http://jsn.shzxlz.cn


<!-- 参考信息 -->