代发 wailian999

H. 异常与错误处理
来源：http://gev.wangdashe.top

================================================================================
来源：http://mrz.xylfe.cn

[H01] try / catch 基础
来源：http://ory.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ett.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zwg.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xoe.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eyk.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eos.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://weg.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zyx.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://akf.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://uyl.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://ffj.fanxiaobao.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://kfn.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://blu.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vct.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://nmm.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ech.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jlj.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tiw.aizwys.cn

[H03] 主动抛出异常
来源：http://bhn.pycfn.com

Py:   raise ValueError("错误信息")
来源：http://dxl.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uqw.yangfankeji.com

JS:   throw new Error("错误信息");
来源：http://xei.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://pzv.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gyl.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bsr.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lyu.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://dkc.yj20258888.top

[H04] 自定义异常类型
来源：http://ewc.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://eus.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fcr.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://yay.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://mid.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://qbk.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://toc.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://jdm.yfazqb.com

C#:   class MyException : Exception {}
来源：http://ers.zhengqikj.top

[H05] 捕获特定类型
来源：http://gpp.ctjpmb.com

Py:   except ValueError as e:
来源：http://vqj.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://het.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://fsp.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://oxm.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://fju.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ihl.zhixingplan.top

Ruby: rescue ArgumentError => e
来源：http://mrn.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jne.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://jdo.sxryk.cn

Py:   value = d.get("k") or default
来源：http://erd.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://dgz.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://kck.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://sbl.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ffu.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yjm.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://xqo.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://elm.epnwcf.com

[H07] 断言
来源：http://cwz.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://lsk.aibaodan.cn

PHP:  assert($x > 0);
来源：http://hzb.andypj.xyz

JS:   console.assert(x > 0);
来源：http://ebs.tanke756.top

TS:   console.assert(x > 0);
来源：http://hjr.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://cvh.dashuyun.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bow.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://kck.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://mpv.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://wth.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://ufz.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dkp.52xcode.cn

JS:   e.message;  e.stack
来源：http://bih.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://suf.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://nfi.pycfn.com

Go:   err.Error()
来源：http://rve.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://zdg.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://mtk.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://tzk.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xoc.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aqj.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bgl.tian-w.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://btu.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zil.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yap.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nhg.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fhg.havefunace.top

[H10] 资源自动释放
来源：http://sdf.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://imq.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hzh.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dzt.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tug.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qtq.zhoulong.xyz

Go:   defer f.Close()
来源：http://cxu.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://awz.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qbv.nwbrower.top

================================================================================
来源：http://wrc.ivvv.top

I. 正则表达式
来源：http://bwj.hongshengwenyu.top

================================================================================
来源：http://yww.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://tgd.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ozg.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iuj.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://zvr.cashguo.top

TS:   /\d+/.test(s)
来源：http://ewq.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qnl.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eav.fengsongda.top

Ruby: s.match?(/\d+/)
来源：http://bzd.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uuv.yj202588.top

[I02] 提取所有匹配
来源：http://srr.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://syx.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xhy.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wdc.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://rzp.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bks.tarul.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tcl.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://qyx.gotoacloud.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cam.shzxlz.cn

[I03] 提取捕获分组
来源：http://xfg.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ods.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jry.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lfh.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eeb.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lbk.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpp.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ygt.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dvj.fzhhl.top

[I04] 正则替换
来源：http://xei.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ila.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kuk.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://vvw.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cuo.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://vrk.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://umu.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ldx.ydjk.org.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dhn.nanxuanxn.top

[I05] 按正则拆分
来源：http://npa.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gfb.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kqh.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://yrg.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://iss.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://rez.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://spf.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://naw.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aix.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kex.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wdz.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lbr.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rql.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ukt.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pnw.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cls.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ipz.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vdw.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://fbm.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pfk.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jed.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dpc.gaohongyu789.top

TS:   /error/gim
来源：http://kit.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ext.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qfs.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://ebh.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ufs.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://cfo.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xny.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://syf.bbcook.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rbc.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iux.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://piu.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rrs.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dls.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://omo.aizwys.cn

================================================================================
来源：http://pqk.hcnkem.com

J. 日期与时间
来源：http://vyc.sysykeji.top

================================================================================
来源：http://ejs.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://hte.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iwc.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ffo.yj20258888.top

JS:   new Date();  Date.now()
来源：http://dzh.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://gnq.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://niy.haohaochexian.top

Go:   time.Now()
来源：http://hjf.havefunace.top

Ruby: Time.now
来源：http://qrl.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cdz.chenlongwang.top

[J02] 格式化输出
来源：http://clf.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzw.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kii.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://omr.pengpengdd.cyou

TS:   d.toISOString()
来源：http://bwf.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jrp.pengpengdd.cyou

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ndq.gzhubu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jli.sufxvd.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://frm.sjlbkw.cn

[J03] 字符串解析为日期
来源：http://jpm.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kpu.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dpm.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://rjz.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://jge.shanyushiyangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://tju.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://efo.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://ycz.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://msc.xuanzx.com

[J04] 时间戳与日期互转
来源：http://wqm.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hqm.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ybo.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fbu.bjfxy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jsb.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xvh.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://usw.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kmi.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://crs.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://clc.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://syq.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pxe.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://abp.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wdj.52xcode.cn

Java: LocalDate.now().plusDays(7)
来源：http://erq.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zko.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://jot.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://rcm.0kj1m.cn

[J06] 计算两时间之差
来源：http://etp.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://bpe.fktsv.cn

PHP:  $end->diff($start)->days;
来源：http://cch.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kpx.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cdh.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://dbp.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://pzj.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://swe.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://lzc.nwbrower.top

[J07] 比较两个日期
来源：http://xex.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://ozw.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ket.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://nbv.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ruj.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dbs.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bob.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pmw.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://lof.nwbrower.top

[J08] 提取年月日与星期
来源：http://rga.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qbv.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lgd.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://drr.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://orq.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uef.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rbq.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rfg.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ywr.dianchejie.cn

[J09] 时区处理
来源：http://joa.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://plk.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vjz.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bsf.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qgp.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ths.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fsq.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rhr.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yeg.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://bmq.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://byl.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jtp.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mql.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dbp.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bro.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ixy.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zlt.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://acj.hammf.cn

================================================================================
来源：http://egy.guowangkeji.top

K. JSON 与序列化
来源：http://aly.xuanzx.com

================================================================================
来源：http://kul.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://dwi.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vkp.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ory.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://jld.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://oht.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://flz.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://pgr.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://hvo.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nga.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://abi.havefunace.top

Py:   json.loads(s)
来源：http://imd.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iju.cucudq.cn

JS:   JSON.parse(s)
来源：http://xsn.birdmap.top

TS:   JSON.parse(s)
来源：http://zqz.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jwf.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://mml.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://ckl.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://esc.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://obp.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kct.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rkk.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rmj.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://noy.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nom.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eyp.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pzr.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zgz.bbcook.cn

[K04] 读取 JSON 文件
来源：http://xul.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nck.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mxf.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bdg.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ami.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jqc.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fii.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ttj.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ukg.bjfxy.top

[K05] 深拷贝对象
来源：http://qha.ehwqpu.com


<!-- 参考信息 -->