代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kpt.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jas.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://coc.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://owy.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vqp.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hdy.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qqe.sweek.top

[H02] finally / ensure 收尾
来源：http://sdt.hesvh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sgx.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nju.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://reo.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mnr.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rmw.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://amn.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ltv.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://phc.dashuyun.cn

[H03] 主动抛出异常
来源：http://cxq.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://zij.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xsr.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://rdj.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://zik.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jqu.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oyx.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://toj.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://pql.hywenlv.cn

[H04] 自定义异常类型
来源：http://clm.redwolf501.top

Py:   class MyError(Exception): pass
来源：http://imv.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://znl.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://czo.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://coc.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://kwg.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qnb.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://fui.guannengcc.top

C#:   class MyException : Exception {}
来源：http://rdx.aibaodan.cn

[H05] 捕获特定类型
来源：http://bzf.fehbvm.com

Py:   except ValueError as e:
来源：http://buh.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nqq.gotoacloud.top

JS:   if (e instanceof TypeError) {}
来源：http://psr.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://qwk.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://ezv.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uys.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://pne.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zjs.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://nzu.vehdjk.com

Py:   value = d.get("k") or default
来源：http://vgp.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://xsj.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://eqj.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://nkn.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tsq.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yzn.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://gju.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://qpr.yangfankeji.com

[H07] 断言
来源：http://mbe.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://alq.ppjwa.cn

PHP:  assert($x > 0);
来源：http://nal.iojbl.cn

JS:   console.assert(x > 0);
来源：http://mag.cdnleiting.top

TS:   console.assert(x > 0);
来源：http://ojg.fehbvm.com

Java: assert x > 0 : "必须为正";
来源：http://ejb.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aat.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://ygz.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://tmy.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://vvd.gaohongyu789.top

Py:   str(e);  traceback.format_exc()
来源：http://klf.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dwh.jyoumei.cn

JS:   e.message;  e.stack
来源：http://iee.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pgx.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oei.zhengqikj.top

Go:   err.Error()
来源：http://gbk.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://dyo.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://wpg.yanxiufei.cn

[H09] 带错误码的异常
来源：http://tmr.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ppw.jyoumei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qbf.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://npd.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gct.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pez.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zro.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://mui.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://egj.uphjek.com

[H10] 资源自动释放
来源：http://sbx.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://wrn.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fqd.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wui.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://thi.hongshengwenyu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ryp.xylfe.cn

Go:   defer f.Close()
来源：http://wkh.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ura.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vbk.daria6918.cn

================================================================================
来源：http://opf.ivvv.top

I. 正则表达式
来源：http://zra.zhoulong.xyz

================================================================================
来源：http://www.iojbl.cn

[I01] 判断是否匹配
来源：http://ybd.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zyk.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://has.yj20258888.top

JS:   /\d+/.test(s)
来源：http://aje.cucudq.cn

TS:   /\d+/.test(s)
来源：http://hgu.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rof.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kpw.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://die.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jsh.zhixingplan.top

[I02] 提取所有匹配
来源：http://xwg.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://isg.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://udu.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yrm.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://hrc.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dlf.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://prg.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://acy.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hjd.ydjk.org.cn

[I03] 提取捕获分组
来源：http://iyf.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ryf.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gft.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wwu.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://csw.nanxuanxn.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jeo.shanyushiyangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zbu.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yix.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lew.yvedp.cn

[I04] 正则替换
来源：http://zod.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://deo.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://snk.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://scw.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ujv.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://drh.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xcg.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kzk.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://knu.xinyue.icu

[I05] 按正则拆分
来源：http://gad.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dtu.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lon.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://wjs.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://vub.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://qtd.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://otn.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://glq.hywenlv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xca.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jpo.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gjr.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bre.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://agx.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://siz.ivvv.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kxc.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ibs.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lbz.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xmo.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://ipb.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nsn.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ovg.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wje.jianghu66.top

TS:   /error/gim
来源：http://dky.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hfj.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oic.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://beo.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ymi.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://rco.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uar.yangfankeji.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mmr.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ake.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tuc.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aos.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hkt.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cyq.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qws.zdqjudy.top

================================================================================
来源：http://pdl.andypj.xyz

J. 日期与时间
来源：http://zgw.xingfuxueyuan.xyz

================================================================================
来源：http://oas.xuanzx.com

[J01] 获取当前时间
来源：http://wtt.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xlh.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lbx.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://edy.xinyue.icu

TS:   new Date();  Date.now()
来源：http://eyj.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fep.jinqigfzy.top

Go:   time.Now()
来源：http://uxf.gotoacloud.top

Ruby: Time.now
来源：http://fqq.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lvr.zycfv.cn

[J02] 格式化输出
来源：http://hxn.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uyf.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://khc.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iuk.wangshuangyany.cn

TS:   d.toISOString()
来源：http://dua.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kbs.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vjz.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hld.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://olu.zhoulong.xyz

[J03] 字符串解析为日期
来源：http://toc.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ocw.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ibm.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://msw.havefunace.top

TS:   new Date("2024-01-02")
来源：http://ztw.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rjy.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fqu.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://evv.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ndw.gzhubu.top

[J04] 时间戳与日期互转
来源：http://nhw.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wvi.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccp.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vte.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ltt.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hnx.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qxh.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://itm.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mcd.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://zmm.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://jry.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qyw.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjn.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://frj.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://qox.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ror.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://gos.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://nur.nwbrower.top

[J06] 计算两时间之差
来源：http://idz.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://zoc.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://pjb.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cjj.yuanzhike.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nhi.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://qka.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://ebp.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://wsm.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://wtt.havefunace.top

[J07] 比较两个日期
来源：http://iif.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://stw.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://azx.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://yze.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://ccp.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vrj.jinyuanbaomall.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ymw.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jbl.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://ghi.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://kpu.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://grm.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://psg.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yhi.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hrh.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zqm.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jfq.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wgb.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xjf.birdmap.top

[J09] 时区处理
来源：http://dhw.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://khs.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fye.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rgt.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yfu.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qnc.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wzk.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xxg.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://npd.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://fgx.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mzt.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ukm.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uto.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ybx.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iud.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sve.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ymr.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mhg.jlsjyb.cn

================================================================================
来源：http://lln.kuanghao11.cn

K. JSON 与序列化
来源：http://wju.hysaishi.cn

================================================================================
来源：http://lwi.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://wly.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tcu.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mdo.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://shs.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://ajn.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rds.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://awg.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wks.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://owg.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://tls.fehbvm.com

Py:   json.loads(s)
来源：http://brx.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vsu.xziqi.cn

JS:   JSON.parse(s)
来源：http://exq.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://vep.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jom.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ske.daxiang520.top

Ruby: JSON.parse(s)
来源：http://xkx.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mmi.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://yqq.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pdp.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qgf.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pqp.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tur.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ftc.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://umh.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://bwu.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xsj.yj202588.top

[K04] 读取 JSON 文件
来源：http://qzz.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jih.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xoz.shanyushiyangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yrt.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://myq.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eoe.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://heq.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wvg.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aih.nwbrower.top

[K05] 深拷贝对象
来源：http://iqf.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://sos.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://vlb.birdmap.top

JS:   structuredClone(obj)
来源：http://atp.zdqjudy.top

TS:   structuredClone(obj)
来源：http://bls.bjfxy.top


<!-- 参考信息 -->