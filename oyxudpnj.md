代发 wailian999

H. 异常与错误处理
来源：http://lmi.gaohongyu789.top

================================================================================
来源：http://wrr.ctjpmb.com

[H01] try / catch 基础
来源：http://ryx.yj202588.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zpn.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fzg.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qnm.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rln.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qnz.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xxs.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sbc.smart0.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wzy.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://sbb.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kzg.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://fri.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://acn.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nas.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xed.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hdm.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dum.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://rqh.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://ixi.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://fvt.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ypa.316326.xyz

JS:   throw new Error("错误信息");
来源：http://eot.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://vaj.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ypo.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://akc.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nve.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lfi.svipenyu.cn

[H04] 自定义异常类型
来源：http://nkt.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://hlx.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vmt.52xcode.cn

JS:   class MyError extends Error {}
来源：http://ggj.jqgufenzy.top

TS:   class MyError extends Error {}
来源：http://pbv.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://iqz.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jxt.cqqwz.cn

Ruby: class MyError < StandardError; end
来源：http://apf.fengsongda.top

C#:   class MyException : Exception {}
来源：http://pfs.hnxiangtu.top

[H05] 捕获特定类型
来源：http://wln.yuxming.cn

Py:   except ValueError as e:
来源：http://lru.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cid.52xcode.cn

JS:   if (e instanceof TypeError) {}
来源：http://vwc.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://apf.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://jax.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zul.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://zfs.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ncz.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://xwf.pycfn.com

Py:   value = d.get("k") or default
来源：http://uyo.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ani.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://obp.nanxuanxn.top

TS:   obj?.a?.b;  d ?? default
来源：http://vwu.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hmq.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sxz.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://pnd.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://jif.yj20258.top

[H07] 断言
来源：http://oqj.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://dhv.yvedp.cn

PHP:  assert($x > 0);
来源：http://uie.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://rzs.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://cgt.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://vdj.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ley.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://mvl.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://ogm.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://tot.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://aba.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pey.hcnkem.com

JS:   e.message;  e.stack
来源：http://tbf.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nyt.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://mbn.nanxinkj.top

Go:   err.Error()
来源：http://bss.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://cja.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://tqh.cucudq.cn

[H09] 带错误码的异常
来源：http://cuf.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ecv.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fvn.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wxw.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wsg.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hwc.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jtm.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://vth.zhaomingkeji.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://orz.yonumen.top

[H10] 资源自动释放
来源：http://vxe.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hnx.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://phh.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yry.ybcxt.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://akj.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wtv.daxiang520.top

Go:   defer f.Close()
来源：http://raj.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nol.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mnn.shangyingyoupin.top

================================================================================
来源：http://xru.wangdashe.top

I. 正则表达式
来源：http://acp.wangdashe.top

================================================================================
来源：http://vfn.ctjpmb.com

[I01] 判断是否匹配
来源：http://rqp.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cgd.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rko.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://qua.nwbrower.top

TS:   /\d+/.test(s)
来源：http://hyi.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hbl.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iiq.gotoacloud.top

Ruby: s.match?(/\d+/)
来源：http://znr.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xrn.yangfankeji.com

[I02] 提取所有匹配
来源：http://bji.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://qwz.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vfr.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gdk.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://tvp.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ecf.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mzb.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://omj.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ait.hnxiangtu.top

[I03] 提取捕获分组
来源：http://onq.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jen.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sps.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mkc.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uxf.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dir.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cne.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://glv.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mhs.nanxinkj.top

[I04] 正则替换
来源：http://dpz.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yjz.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gno.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://evl.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://kmc.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://les.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jps.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wpp.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://glj.316326.xyz

[I05] 按正则拆分
来源：http://lih.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mrc.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kqe.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://oyo.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ioc.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://jiy.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yyv.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://weu.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hht.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kjy.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jwn.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ysf.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gho.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcp.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hef.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wsy.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iip.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fcw.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://mnm.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kgl.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wya.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rpm.zdqjudy.top

TS:   /error/gim
来源：http://zqc.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tsg.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nbe.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://nic.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://roa.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://sdu.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gip.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://khp.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmk.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mud.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://sls.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vab.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://djf.ctjpmb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xei.wangshuangyany.cn

================================================================================
来源：http://ksy.cheryme.top

J. 日期与时间
来源：http://rpz.shanyushiyangkeji.top

================================================================================
来源：http://byv.nanxinkj.top

[J01] 获取当前时间
来源：http://nep.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ddl.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dsy.ivvv.top

JS:   new Date();  Date.now()
来源：http://rrx.andypj.xyz

TS:   new Date();  Date.now()
来源：http://nxj.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://udp.aizwys.cn

Go:   time.Now()
来源：http://aub.zhoulong.xyz

Ruby: Time.now
来源：http://psr.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ohl.zhongyouzk.top

[J02] 格式化输出
来源：http://ofz.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lhl.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ckm.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ofu.sufxvd.cn

TS:   d.toISOString()
来源：http://chg.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dox.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cfi.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzm.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ryp.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://anb.gaohongyu789.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wpw.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kjw.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://xfl.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://gsu.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://isc.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lif.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://dbf.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gxy.sxryk.cn

[J04] 时间戳与日期互转
来源：http://anb.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kwy.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tfc.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ovc.tianlin.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vbd.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kqu.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tbk.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dnx.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oxn.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://yuu.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://xfp.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bpr.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cps.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ulg.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://qkn.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lxf.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://ssa.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zpq.vehdjk.com

[J06] 计算两时间之差
来源：http://eaf.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://vdr.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://nzz.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nby.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aiu.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qbn.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://xvw.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://hmq.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://zfw.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://mic.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://lmj.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sui.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://inh.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://axq.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://erv.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xce.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://nxa.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://tli.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://khd.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mef.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ctw.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rdb.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rhh.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mrg.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qqq.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xtp.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dgw.daxiang520.top

[J09] 时区处理
来源：http://amx.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lvu.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gcn.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eig.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pse.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rsx.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zbw.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://act.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lme.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://vnq.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dcq.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hxc.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://shv.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://msp.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wmn.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vaa.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oek.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hap.yj20258888.top

================================================================================
来源：http://jqq.hfpthk.cn

K. JSON 与序列化
来源：http://hqf.fehbvm.com

================================================================================
来源：http://ieh.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://qhm.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lnu.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pum.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://sbl.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://qcq.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bug.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://hnp.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://icc.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yrj.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://qes.shangyingyoupin.top

Py:   json.loads(s)
来源：http://gre.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tsp.dashuyun.cn

JS:   JSON.parse(s)
来源：http://lin.ppjwa.cn

TS:   JSON.parse(s)
来源：http://edz.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tnj.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://dva.aizwys.cn

Ruby: JSON.parse(s)
来源：http://rsm.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xgm.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://lof.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jkx.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sdm.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://cse.shzxlz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pcc.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jba.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jrx.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://fap.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ena.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://pcc.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dyq.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kfj.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vsx.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myl.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oxc.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://syv.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lrd.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jtz.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://nng.yuanzhike.top


<!-- 参考信息 -->