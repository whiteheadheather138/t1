代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aio.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iji.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qyt.xinyue.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ggc.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kzy.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gsy.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mzz.sysykeji.top

[H02] finally / ensure 收尾
来源：http://jbq.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://bcz.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mxf.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ivl.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aww.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sgz.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fgu.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gzs.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://api.hnxiangtu.top

[H03] 主动抛出异常
来源：http://dgg.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://dtv.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jhy.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://pld.xuetiantiany.cn

TS:   throw new Error("错误信息");
来源：http://eww.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lct.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hnl.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xrm.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://bvu.fehbvm.com

[H04] 自定义异常类型
来源：http://dox.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://vkn.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://thn.jianghu66.top

JS:   class MyError extends Error {}
来源：http://lwj.wangdashe.top

TS:   class MyError extends Error {}
来源：http://euq.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://znh.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cen.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://arq.hesvh.cn

C#:   class MyException : Exception {}
来源：http://mht.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://ycu.fehbvm.com

Py:   except ValueError as e:
来源：http://eoc.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pkb.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://ekz.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://zel.yangfankeji.com

Java: catch (IOException | SQLException e) {}
来源：http://hkc.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xpx.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://lln.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ebg.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://xze.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://qha.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://dih.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://qny.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ubk.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mob.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ppp.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://uel.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://leq.hnqzz.top

[H07] 断言
来源：http://puk.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://vyg.hammf.cn

PHP:  assert($x > 0);
来源：http://pom.yongpay.top

JS:   console.assert(x > 0);
来源：http://kbk.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://qaq.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://lmy.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yeh.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ojv.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://vne.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://xxa.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://eas.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fqb.fengsongda.top

JS:   e.message;  e.stack
来源：http://tys.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hxr.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://puu.hysaishi.cn

Go:   err.Error()
来源：http://nul.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://bax.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://wmf.hywenlv.cn

[H09] 带错误码的异常
来源：http://jjx.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uvz.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nsp.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://apb.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://djj.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lzu.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uaz.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mei.nanxinkj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://esh.shzxlz.cn

[H10] 资源自动释放
来源：http://ast.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://qjt.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tzd.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hfm.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mch.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qcw.mhx1999.top

Go:   defer f.Close()
来源：http://ahq.xuetiantiany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cvx.zhijiandao.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fyx.yj20258888.top

================================================================================
来源：http://mer.meibo888.top

I. 正则表达式
来源：http://uwr.cqqwz.cn

================================================================================
来源：http://ukx.hfpthk.cn

[I01] 判断是否匹配
来源：http://isg.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://trb.haohaochexian.top

PHP:  preg_match('/\d+/', $s);
来源：http://glt.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://sby.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://xce.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fxt.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zob.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://toz.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://izx.zhongyouzk.top

[I02] 提取所有匹配
来源：http://pld.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://rgk.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yvp.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mka.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://mdr.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ivn.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tro.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://hnc.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vvw.tianlin.xyz

[I03] 提取捕获分组
来源：http://tuw.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wye.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sub.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ame.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ufa.zhongyouzk.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yeu.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cdu.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qxm.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lfo.uphjek.com

[I04] 正则替换
来源：http://dcy.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uoj.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mcw.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lri.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://djx.hesvh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xly.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vfl.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jvi.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eya.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://nfr.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fmm.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://urg.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://vmw.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://pfp.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://dnu.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lgm.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sdq.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lqe.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bjm.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kja.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://spp.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nvu.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dtc.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yxu.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pqm.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wky.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://viu.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://vry.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ybf.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://usl.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aog.yangfankeji.com

TS:   /error/gim
来源：http://eou.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wpy.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xrp.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://nho.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lte.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://jqt.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ocb.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mep.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://okn.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qzw.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yxe.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mba.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qfo.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fkx.havefunace.top

================================================================================
来源：http://cqs.zdbjq.cn

J. 日期与时间
来源：http://ikr.hysaishi.cn

================================================================================
来源：http://vez.cqqwz.cn

[J01] 获取当前时间
来源：http://mal.vehdjk.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://dhe.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ssv.aizwys.cn

JS:   new Date();  Date.now()
来源：http://tni.havefunace.top

TS:   new Date();  Date.now()
来源：http://yza.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ltb.hesvh.cn

Go:   time.Now()
来源：http://aid.fanxiaobao.xyz

Ruby: Time.now
来源：http://hwu.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vpb.birdmap.top

[J02] 格式化输出
来源：http://zxw.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kii.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://avl.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vjv.cucudq.cn

TS:   d.toISOString()
来源：http://qka.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://exq.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://are.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qkh.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rom.nanxinkj.top

[J03] 字符串解析为日期
来源：http://ugu.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yqj.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://azk.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://viy.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://pet.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://gkt.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://evy.jinqigfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://qpc.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cqo.sxryk.cn

[J04] 时间戳与日期互转
来源：http://non.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://voj.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aye.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blg.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://wly.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bju.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ige.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bxv.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ioe.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://scy.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://hyq.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dkl.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xgr.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pxl.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://vqx.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ojy.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://qli.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://fvo.hnqzz.top

[J06] 计算两时间之差
来源：http://pvn.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://lsp.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://hln.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xdo.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gsq.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://rka.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://lhi.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://bae.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://bfu.316326.xyz

[J07] 比较两个日期
来源：http://edt.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://val.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uip.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xbz.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://trr.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qwe.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aeb.hywenlv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jrt.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://gif.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://isq.yj20258.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ktk.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blu.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kgt.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ube.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wly.bjfxy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hrn.jqgfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://emn.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pay.xuetiantiany.cn

[J09] 时区处理
来源：http://gzz.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fso.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qhl.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yov.0kj1m.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ymr.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hpr.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nyu.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://apg.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cgw.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://lfk.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zsx.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bbe.feifeiyinyue.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://osw.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fri.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jxg.yj202588.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mgu.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mnc.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jdv.hysaishi.cn

================================================================================
来源：http://uip.yj202588.top

K. JSON 与序列化
来源：http://gfl.bjfxy.top

================================================================================
来源：http://eyo.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://ajp.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ojw.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iio.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://xnp.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://ldd.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xoy.xylfe.cn

Go:   json.Marshal(obj)
来源：http://col.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nxr.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jeq.zhiwuduotai.top

[K02] JSON 字符串转对象
来源：http://jie.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://ehh.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzg.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://yys.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://sez.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xap.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://jgy.ivvv.top

Ruby: JSON.parse(s)
来源：http://fwo.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wcw.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://tjz.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dhr.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zip.jqgufenzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jge.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wxk.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mjz.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lpk.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://gtx.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cwp.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://jgo.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sah.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ykb.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nyv.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hvq.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://egj.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eux.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://oqr.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jmm.shuidangran.top

[K05] 深拷贝对象
来源：http://bwz.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://ixv.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://hlk.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://phc.jianghu66.top

TS:   structuredClone(obj)
来源：http://gdz.sysykeji.top


<!-- 参考信息 -->