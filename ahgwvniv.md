代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://vmq.yongpay.top

Ruby: obj.instance_variables
来源：http://olf.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://rjm.0kj1m.cn

================================================================================
来源：http://gwk.jinghuilouyu.cn

H. 异常与错误处理
来源：http://hlr.aizwys.cn

================================================================================
来源：http://xww.meibo888.top

[H01] try / catch 基础
来源：http://vuk.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uth.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gpp.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ngb.nanxuanxn.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nky.fanxiaobao.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://slq.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jel.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://giu.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jpv.aibaodan.cn

[H02] finally / ensure 收尾
来源：http://vrf.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mlf.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://lds.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kly.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gvf.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://unn.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ptw.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://tgf.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://wvl.xziqi.cn

[H03] 主动抛出异常
来源：http://zkt.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://wur.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hcm.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://dff.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://rai.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lmf.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ajf.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://kaz.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://fao.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://ncl.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://ycr.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bkg.yongpay.top

JS:   class MyError extends Error {}
来源：http://ycz.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://mcl.xuetiantiany.cn

Java: class MyException extends RuntimeException {}
来源：http://cmg.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aan.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://qey.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://chx.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://uyx.hammf.cn

Py:   except ValueError as e:
来源：http://asy.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ebk.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://wix.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://uqa.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://gru.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kez.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://vsy.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sqs.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://qsx.birdmap.top

Py:   value = d.get("k") or default
来源：http://saf.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://yip.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bhe.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bih.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vdj.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zev.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://amh.dashuyun.cn

C#:   obj?.A?.B ?? default
来源：http://tph.iojbl.cn

[H07] 断言
来源：http://tua.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://dyh.uphjek.com

PHP:  assert($x > 0);
来源：http://pma.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://pdd.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://gum.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://fkv.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fpb.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xrc.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://upn.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://xwv.316326.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ssm.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wmz.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://qyo.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jaf.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ncw.aibaodan.cn

Go:   err.Error()
来源：http://ohz.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://kqo.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://gtp.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://xdh.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jgt.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://asn.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pty.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xfh.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mwx.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ttr.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://upz.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mhb.wangshuangyany.cn

[H10] 资源自动释放
来源：http://ofu.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nxj.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gil.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qai.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mga.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tsa.sjlbkw.cn

Go:   defer f.Close()
来源：http://huh.dianchejie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pfd.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bpb.chenzaomai.com

================================================================================
来源：http://gia.zhaomingkeji.xyz

I. 正则表达式
来源：http://rog.ctjpmb.com

================================================================================
来源：http://hwe.tianlin.xyz

[I01] 判断是否匹配
来源：http://vgn.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tvp.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://rpb.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://cgo.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://put.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vde.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ppz.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://nbw.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bcp.hfpthk.cn

[I02] 提取所有匹配
来源：http://xqw.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://zjz.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://udq.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://doz.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://xgl.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sck.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://avr.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://apu.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qdb.chenlongwang.top

[I03] 提取捕获分组
来源：http://znr.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qnt.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://asy.daxiang520.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vxq.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hig.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ztw.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rsk.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wzy.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xeb.hcnkem.com

[I04] 正则替换
来源：http://bwa.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sdv.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wkx.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://rrk.hcnkem.com

TS:   s.replace(/\d+/g, "#")
来源：http://phv.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://exl.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bno.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gfd.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hko.gotoacloud.top

[I05] 按正则拆分
来源：http://jzk.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uaf.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oea.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://weh.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://yjg.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://txv.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://myq.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://vtg.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bmj.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gvu.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mie.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uvk.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wom.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vss.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pol.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://avn.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xwx.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xxz.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://vtr.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jxx.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yfu.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://znm.yj20258.top

TS:   /error/gim
来源：http://dcg.cheryme.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rkw.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cci.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://hfj.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ctn.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://viy.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dxt.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ndl.vqdsnc.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pyp.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tng.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zbr.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rtm.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vvg.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://adl.tarul.cn

================================================================================
来源：http://ixq.zdqjudy.top

J. 日期与时间
来源：http://fca.chenzaomai.com

================================================================================
来源：http://oml.aizwys.cn

[J01] 获取当前时间
来源：http://ohw.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hsd.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fxc.bbcook.cn

JS:   new Date();  Date.now()
来源：http://yva.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://xrt.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ozd.jqgfzy.top

Go:   time.Now()
来源：http://akw.shzxlz.cn

Ruby: Time.now
来源：http://ood.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vte.hnxiangtu.top

[J02] 格式化输出
来源：http://ohl.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qjt.xinyue.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fkb.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ojr.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://dvu.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ivr.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wrb.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tlg.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fzo.tianlin.xyz

[J03] 字符串解析为日期
来源：http://zyb.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jsb.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jod.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://usa.yj20258.top

TS:   new Date("2024-01-02")
来源：http://iwf.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://bjx.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qps.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://jcf.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wmd.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://qjv.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://diy.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://miv.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lpa.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gbs.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cct.cheryme.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ytq.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gww.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mvw.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://tkx.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://ecq.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cyv.sysykeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xhe.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bga.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://aqs.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nak.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://iuf.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://jhh.ehwqpu.com

[J06] 计算两时间之差
来源：http://myp.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://hwm.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://rlc.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mxh.gzhubu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cpc.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://klr.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://afb.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://lmz.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://xsb.sysykeji.top

[J07] 比较两个日期
来源：http://fhj.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://sod.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eba.aizwys.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xxr.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://qpe.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rdo.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ivn.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xkk.nanxinkj.top

C#:   d1 < d2;  d1 == d2
来源：http://jtj.hysaishi.cn

[J08] 提取年月日与星期
来源：http://jpm.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://woa.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yiw.feifeiyinyue.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ryd.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gdr.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xuk.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qxv.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zgx.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lue.chenzaomai.com

[J09] 时区处理
来源：http://oih.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uxp.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rrr.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gnr.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://igv.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wvd.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://djw.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ibd.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://adh.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://luq.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tdk.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tzl.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://grf.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ehr.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qhu.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jdn.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nho.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eef.tanke756.top

================================================================================
来源：http://llw.dianchejie.cn

K. JSON 与序列化
来源：http://kxx.svipenyu.cn

================================================================================
来源：http://fws.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://sxw.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://abo.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xnh.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://kin.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://wir.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kgv.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://tdu.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ssb.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://son.ybcxt.top

[K02] JSON 字符串转对象
来源：http://bqc.cdnleiting.top

Py:   json.loads(s)
来源：http://jci.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zqi.yvedp.cn

JS:   JSON.parse(s)
来源：http://nvz.zhixingplan.top

TS:   JSON.parse(s)
来源：http://sko.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nqw.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://oqg.iojbl.cn

Ruby: JSON.parse(s)
来源：http://lwy.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://esk.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://gds.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jnz.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ubo.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://tku.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uvo.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zwz.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jpd.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://djx.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jmv.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://abz.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://knj.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wqb.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hxy.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gml.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hsc.vehdjk.com


<!-- 参考信息 -->