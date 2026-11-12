代发 wailian999

[H03] 主动抛出异常
来源：http://hgz.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://fze.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jrh.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://bav.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://jww.zhixingplan.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qcz.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gkc.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mnr.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://mqy.sjlbkw.cn

[H04] 自定义异常类型
来源：http://jlt.hcnkem.com

Py:   class MyError(Exception): pass
来源：http://uzd.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://thh.bjfxy.top

JS:   class MyError extends Error {}
来源：http://cpi.cucudq.cn

TS:   class MyError extends Error {}
来源：http://rei.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://wju.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ska.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://bbw.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://tlr.iojbl.cn

[H05] 捕获特定类型
来源：http://luh.xuanzx.com

Py:   except ValueError as e:
来源：http://yos.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nex.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://qlu.zhixingplan.top

TS:   if (e instanceof TypeError) {}
来源：http://wun.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://hps.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tyc.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://vgw.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rae.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://eoy.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://rlu.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://jxk.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kuj.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://csh.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xci.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tyh.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://wlg.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://vfi.jinqigfzy.top

[H07] 断言
来源：http://vsb.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://pog.gaohongyu789.top

PHP:  assert($x > 0);
来源：http://dze.xuanzx.com

JS:   console.assert(x > 0);
来源：http://fvs.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://bkg.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://wyd.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nsj.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bff.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://tup.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://vvc.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://ygo.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ljb.xuetiantiany.cn

JS:   e.message;  e.stack
来源：http://lfv.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://liw.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://olh.iojbl.cn

Go:   err.Error()
来源：http://gcj.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://jso.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://uaf.ivvv.top

[H09] 带错误码的异常
来源：http://hai.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gst.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ldq.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eio.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xoj.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://anj.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iaa.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://wnt.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nmi.jiagoushi.top

[H10] 资源自动释放
来源：http://ppa.tarul.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xnx.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bse.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ozd.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nxt.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vbj.zdqjudy.top

Go:   defer f.Close()
来源：http://cpg.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kxn.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sif.nwbrower.top

================================================================================
来源：http://uep.guowangkeji.top

I. 正则表达式
来源：http://znf.xingfuxueyuan.xyz

================================================================================
来源：http://wlg.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://hmd.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jwx.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://esm.xziqi.cn

JS:   /\d+/.test(s)
来源：http://gjn.zycfv.cn

TS:   /\d+/.test(s)
来源：http://ava.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hst.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dom.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://vns.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sah.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://abq.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://cip.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ttk.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ewx.gotoacloud.top

TS:   s.match(/\d+/g)
来源：http://qym.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gpz.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cer.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://mzh.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gmx.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://ziy.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wjh.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vro.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vjj.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jwb.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ltk.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hjn.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://czw.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vkp.dianchejie.cn

[I04] 正则替换
来源：http://zjs.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rks.bjfxy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nnh.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://voy.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zxl.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xgc.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://axr.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rxl.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mmr.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://qwp.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bze.wangdashe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kqj.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://nhr.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://aqw.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://kcy.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bug.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://ymn.zhixingplan.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://afv.aizwys.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fhd.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wgu.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pqb.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jnw.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rjy.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wta.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oqz.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ypf.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://frg.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://lwe.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://inu.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fnd.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yqr.yangfankeji.com

TS:   /error/gim
来源：http://nym.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bfa.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://egj.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://mfg.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yoj.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://xki.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kuo.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://twi.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ivc.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://efw.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lfh.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xjv.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gpd.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://myt.shangyingyoupin.top

================================================================================
来源：http://ynb.redwolf501.top

J. 日期与时间
来源：http://koi.ctjpmb.com

================================================================================
来源：http://ngm.hywenlv.cn

[J01] 获取当前时间
来源：http://nuc.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fih.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wdv.meibo888.top

JS:   new Date();  Date.now()
来源：http://jgq.fengsongda.top

TS:   new Date();  Date.now()
来源：http://kdy.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bvb.yuanzhike.top

Go:   time.Now()
来源：http://agr.snrcjt.cn

Ruby: Time.now
来源：http://trh.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ycp.jyoumei.cn

[J02] 格式化输出
来源：http://znw.0kj1m.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://whj.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zvz.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sxk.haohaochexian.top

TS:   d.toISOString()
来源：http://suc.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://deh.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lzx.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://guf.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pya.zdqjudy.top

[J03] 字符串解析为日期
来源：http://mqz.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jaf.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nei.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://ita.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://yko.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://tgp.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jfs.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://hhx.ivvv.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mfs.ivvv.top

[J04] 时间戳与日期互转
来源：http://luf.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dkx.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ags.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zlw.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://gty.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uxg.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dyw.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hxo.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nou.zhixingplan.top

[J05] 时间加减（加 7 天）
来源：http://mwn.tarul.cn

Py:   now + timedelta(days=7)
来源：http://hiz.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xuh.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fqy.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gby.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://vzf.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qbo.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://qjs.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sgq.zhongyouzk.top

[J06] 计算两时间之差
来源：http://rab.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://slq.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://nwr.ppjwa.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cgt.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bfe.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://kec.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://bja.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://imd.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://rbd.sysykeji.top

[J07] 比较两个日期
来源：http://ary.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://msg.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ckt.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://oae.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://euw.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qgd.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://unp.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://acj.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://pil.jinqigufen.top

[J08] 提取年月日与星期
来源：http://ehj.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yog.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://isd.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ysx.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rug.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pjk.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://omp.dashuyun.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ehe.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ukg.feifeiyinyue.top

[J09] 时区处理
来源：http://iht.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hvb.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ioa.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kux.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jry.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oht.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cnw.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zgh.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hht.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://ztp.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lpv.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://meh.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sft.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yev.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://swx.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jas.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://boq.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vlr.hongshengwenyu.top

================================================================================
来源：http://rvd.316326.xyz

K. JSON 与序列化
来源：http://zuy.ivvv.top

================================================================================
来源：http://mvi.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://kiu.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://svr.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sad.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://uug.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://vbg.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oon.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://gvz.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bur.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://upi.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://idj.gotoacloud.top

Py:   json.loads(s)
来源：http://txy.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://brs.guowangkeji.top

JS:   JSON.parse(s)
来源：http://lgg.yfazqb.com

TS:   JSON.parse(s)
来源：http://dfr.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wwe.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://oct.hammf.cn

Ruby: JSON.parse(s)
来源：http://lpm.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gcs.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://nfj.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xns.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rtv.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://toy.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mro.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://alh.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mea.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xhx.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ldj.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://crv.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fnu.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hvc.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kxa.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sot.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fpg.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zjv.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gsm.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zst.svipenyu.cn

[K05] 深拷贝对象
来源：http://enq.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://uuz.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://vrk.yuxming.cn

JS:   structuredClone(obj)
来源：http://fgl.birdmap.top

TS:   structuredClone(obj)
来源：http://djg.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sza.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fhn.fanxiaobao.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yyc.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lhw.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://jux.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eyn.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bfw.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://myd.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yyy.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gto.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nap.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://grl.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yrk.ehwqpu.com

[K07] 进制转换
来源：http://ezs.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jfi.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qyh.xylfe.cn


<!-- 参考信息 -->