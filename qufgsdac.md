代发 wailian999

H. 异常与错误处理
来源：http://asd.jlsjyb.cn

================================================================================
来源：http://ias.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://dbx.jinqigufen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eja.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dqa.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://liu.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ydz.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mom.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dcm.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tvk.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://odp.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://njo.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rww.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lrv.chenjidiqi.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://loe.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dye.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://qhr.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nqa.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wkh.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ysm.ppjwa.cn

[H03] 主动抛出异常
来源：http://wul.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://sai.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rsr.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://beo.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://avf.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vxg.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ugd.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ozy.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eoh.fengsongda.top

[H04] 自定义异常类型
来源：http://zzu.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://pgv.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://alp.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://nnq.ivvv.top

TS:   class MyError extends Error {}
来源：http://zro.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://qea.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jbv.52xcode.cn

Ruby: class MyError < StandardError; end
来源：http://zqp.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://hii.ydjk.org.cn

[H05] 捕获特定类型
来源：http://iiz.nanxuanxn.top

Py:   except ValueError as e:
来源：http://nbp.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dpd.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://yha.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://dex.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://lvi.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ynk.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://bwe.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wcu.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://xik.guannengcc.top

Py:   value = d.get("k") or default
来源：http://nly.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gtr.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://fjk.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ads.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ult.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rae.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://qdv.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://kpv.jqgufenzy.top

[H07] 断言
来源：http://xlv.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://jwg.dianchejie.cn

PHP:  assert($x > 0);
来源：http://xjt.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://tri.bjfxy.top

TS:   console.assert(x > 0);
来源：http://cag.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://mux.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xhc.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://zom.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://yah.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://plv.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://hhx.xuetiantiany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bfe.316326.xyz

JS:   e.message;  e.stack
来源：http://xdo.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gnq.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://hsu.kuanghao11.cn

Go:   err.Error()
来源：http://hoo.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://iex.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://ppk.cqqwz.cn

[H09] 带错误码的异常
来源：http://zar.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bug.0kj1m.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwg.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ahv.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nfn.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://knt.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vfk.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://cfc.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jkl.yuanzhike.top

[H10] 资源自动释放
来源：http://huf.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qxm.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iyl.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://psv.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vjn.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hlw.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://wxe.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lda.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://igs.snrcjt.cn

================================================================================
来源：http://oya.bjfxy.top

I. 正则表达式
来源：http://hbv.birdmap.top

================================================================================
来源：http://nse.316326.xyz

[I01] 判断是否匹配
来源：http://lgo.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rky.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mpx.ybcxt.top

JS:   /\d+/.test(s)
来源：http://owh.redwolf501.top

TS:   /\d+/.test(s)
来源：http://buh.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kfh.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sfk.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://ehw.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xwi.chenlongwang.top

[I02] 提取所有匹配
来源：http://gcu.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://xnp.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cia.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mum.sweek.top

TS:   s.match(/\d+/g)
来源：http://vtb.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fuy.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dty.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://osu.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cbk.hnxiangtu.top

[I03] 提取捕获分组
来源：http://kde.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zkq.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tmu.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rms.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xbf.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nou.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wde.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pcr.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fsf.jinqigfzy.top

[I04] 正则替换
来源：http://vfb.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lig.0kj1m.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zzr.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://pwn.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://fxb.ybcxt.top

Java: s.replaceAll("\\d+", "#")
来源：http://vdz.hnxiangtu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vvg.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xjs.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xbo.smart0.xyz

[I05] 按正则拆分
来源：http://pdw.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://inh.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hme.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://xva.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://rwu.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://fhd.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uzf.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://dkc.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rlf.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://otd.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gju.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://odr.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wns.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zqd.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lgs.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://teb.zhongyouzk.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mww.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://udx.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://gri.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qiu.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tei.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ccs.xuanzx.com

TS:   /error/gim
来源：http://cje.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jpg.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tzi.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://whr.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kvn.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://mdz.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zka.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sig.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://avj.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqo.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ruc.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://roo.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uus.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://itg.vehdjk.com

================================================================================
来源：http://jig.zhixingplan.top

J. 日期与时间
来源：http://czs.zhixingplan.top

================================================================================
来源：http://yyv.dianchejie.cn

[J01] 获取当前时间
来源：http://axr.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://frd.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://icu.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://tru.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://lsq.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lnv.shanyushiyangkeji.top

Go:   time.Now()
来源：http://joj.yuxming.cn

Ruby: Time.now
来源：http://qkv.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aei.sufxvd.cn

[J02] 格式化输出
来源：http://yfu.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qnv.zdbjq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nhk.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://otm.jianghu66.top

TS:   d.toISOString()
来源：http://kmz.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jzj.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xez.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hqj.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ztf.shzxlz.cn

[J03] 字符串解析为日期
来源：http://jxu.zhoulong.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jvl.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pna.ybcxt.top

JS:   new Date("2024-01-02")
来源：http://gld.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://lwd.ydzc1.top

Java: LocalDate.parse("2024-01-02")
来源：http://yps.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nep.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://zzs.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gcb.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://bic.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xmq.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://acu.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://afb.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iot.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xpx.hesvh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://czp.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://phs.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mto.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://ijg.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://hre.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vtd.c1oappe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://opg.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uju.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://xkq.zhengqikj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ggn.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://nzf.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ims.xylfe.cn

[J06] 计算两时间之差
来源：http://cdh.hammf.cn

Py:   (end - start).total_seconds()
来源：http://pcz.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://ihk.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nqj.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xaw.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://map.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://txa.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://lxh.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://ivc.ppjwa.cn

[J07] 比较两个日期
来源：http://skv.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://ymp.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uhn.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://agv.yvedp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nue.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://syr.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://shz.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://onb.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://chr.c1oappe.top

[J08] 提取年月日与星期
来源：http://qce.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qid.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mex.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rvg.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kxu.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vcu.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mpa.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pkr.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ecc.kuanghao11.cn

[J09] 时区处理
来源：http://cvc.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://adn.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vbn.dianchejie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opa.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yqx.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bpr.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mgf.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tmp.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wbi.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://loy.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jam.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gmd.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gqs.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jvd.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qmg.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bhu.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wwa.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fve.jlsjyb.cn

================================================================================
来源：http://srn.gogol.net.cn

K. JSON 与序列化
来源：http://dpb.0kj1m.cn

================================================================================
来源：http://gtw.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://jpm.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cea.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cec.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://bgf.wangdashe.top

TS:   JSON.stringify(obj)
来源：http://xuk.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://deb.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://ejy.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://vjd.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://drk.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://liz.hongshengwenyu.top

Py:   json.loads(s)
来源：http://ftb.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mrk.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://ley.316326.xyz

TS:   JSON.parse(s)
来源：http://dte.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eic.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://gqr.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://edz.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pme.xingfuxueyuan.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ftk.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aov.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zhv.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://teu.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://duw.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cwh.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://odl.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://afs.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://esj.yonumen.top

[K04] 读取 JSON 文件
来源：http://dte.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cvh.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qsf.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvj.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gac.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gvf.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oif.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zmj.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oce.gzhubu.top

[K05] 深拷贝对象
来源：http://ogh.sysykeji.top


<!-- 参考信息 -->