代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tlf.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vwl.yangfankeji.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qmu.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qoi.andypj.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qqp.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lqb.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xlc.yj202588.top

[H02] finally / ensure 收尾
来源：http://mim.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://lag.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kum.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rdp.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bpe.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gif.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://mvq.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uct.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kfx.gaohongyu789.top

[H03] 主动抛出异常
来源：http://lro.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://mne.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fqo.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://wiy.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://qzp.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mem.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kaw.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tpq.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://hli.yj20258888.top

[H04] 自定义异常类型
来源：http://enx.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://bnk.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://gag.fzhhl.top

JS:   class MyError extends Error {}
来源：http://akw.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://bis.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://zif.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eay.cashguo.top

Ruby: class MyError < StandardError; end
来源：http://wao.guannengcc.top

C#:   class MyException : Exception {}
来源：http://wkd.zhixingplan.top

[H05] 捕获特定类型
来源：http://rxx.xylfe.cn

Py:   except ValueError as e:
来源：http://tmj.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zic.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://nwf.wangdashe.top

TS:   if (e instanceof TypeError) {}
来源：http://lgz.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://hig.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gfs.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://gky.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cfs.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://mcw.hcnkem.com

Py:   value = d.get("k") or default
来源：http://try.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rqb.tanke756.top

JS:   obj?.a?.b;  d ?? default
来源：http://vfv.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://xrs.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kah.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rvi.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://iay.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://jmn.feifeiyinyue.top

[H07] 断言
来源：http://jrs.jqgfzy.top

Py:   assert x > 0, "必须为正"
来源：http://rgi.9152youxi.cn

PHP:  assert($x > 0);
来源：http://wpr.ybcxt.top

JS:   console.assert(x > 0);
来源：http://ory.birdmap.top

TS:   console.assert(x > 0);
来源：http://vlw.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://mwy.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tmp.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xet.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://xwh.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://xxw.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://fgx.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://apx.wangdashe.top

JS:   e.message;  e.stack
来源：http://thj.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hug.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kzy.daria6918.cn

Go:   err.Error()
来源：http://lpy.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://nsb.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://wkt.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://ikj.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gvs.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wdx.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ves.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tiq.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://trx.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hny.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uhg.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://tnc.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://idy.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zwv.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zcy.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ixb.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kzh.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vgo.cucudq.cn

Go:   defer f.Close()
来源：http://qjo.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kgd.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sip.yj202588.top

================================================================================
来源：http://qra.yonumen.top

I. 正则表达式
来源：http://mzc.smart0.xyz

================================================================================
来源：http://nru.yj20258888.top

[I01] 判断是否匹配
来源：http://xwf.gaohongyu789.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tli.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://bwm.vehdjk.com

JS:   /\d+/.test(s)
来源：http://dtf.wangshuangyany.cn

TS:   /\d+/.test(s)
来源：http://dct.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lmj.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zlw.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://qga.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tyd.ydjk.org.cn

[I02] 提取所有匹配
来源：http://pcy.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://rub.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qgt.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://brn.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://xtj.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://efq.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://unk.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://ccw.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://svk.zdqjudy.top

[I03] 提取捕获分组
来源：http://rqb.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://feh.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xlh.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://emn.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ena.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cav.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://faf.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oks.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zkp.jianghu66.top

[I04] 正则替换
来源：http://dwa.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kjx.gzhubu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wms.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://bfi.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://tfa.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lht.nwbrower.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lds.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ump.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kdw.nanxuanxn.top

[I05] 按正则拆分
来源：http://prb.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lzx.fzhhl.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vlh.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://zwy.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://vxu.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://ngb.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kyr.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://cdn.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uhy.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://luu.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xnu.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hso.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hld.ydjk.org.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kij.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bxa.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pjv.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nhd.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kzy.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://ftf.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fqa.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ilb.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mob.cqqwz.cn

TS:   /error/gim
来源：http://kwt.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://avd.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qse.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://cke.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lfe.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://mxa.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lnz.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://feh.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nra.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://veu.zhiwuduotai.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uuz.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://puc.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qcf.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cpd.yvedp.cn

================================================================================
来源：http://ast.xylfe.cn

J. 日期与时间
来源：http://gum.yj202588.top

================================================================================
来源：http://hnq.yangfankeji.com

[J01] 获取当前时间
来源：http://fls.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dlr.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://foo.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://tig.ybcxt.top

TS:   new Date();  Date.now()
来源：http://lhm.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://awn.ehwqpu.com

Go:   time.Now()
来源：http://bzw.zhoulong.xyz

Ruby: Time.now
来源：http://cqv.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fjf.xinyue.icu

[J02] 格式化输出
来源：http://vrq.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hgm.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gvh.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rrm.vqdsnc.cn

TS:   d.toISOString()
来源：http://tcj.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://usz.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gup.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dzn.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vxm.birdmap.top

[J03] 字符串解析为日期
来源：http://oqm.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bsj.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zac.yj202588.top

JS:   new Date("2024-01-02")
来源：http://ifh.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://rzi.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://edk.andypj.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yex.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://oie.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://omn.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://wfu.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ikk.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sjf.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xhs.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://zcy.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cvq.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gsy.sufxvd.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://awu.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jgn.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://lbr.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://wnb.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://anc.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qdu.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rpv.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://pyl.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ouf.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://kmq.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://jet.svipenyu.cn

[J06] 计算两时间之差
来源：http://qld.cucudq.cn

Py:   (end - start).total_seconds()
来源：http://eku.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://uwn.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aui.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lzr.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://qgx.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://lkv.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://nmw.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://jer.hesvh.cn

[J07] 比较两个日期
来源：http://uty.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://joj.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lej.ivvv.top

JS:   d1.getTime() < d2.getTime()
来源：http://sfe.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://txp.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fry.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ekj.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://mat.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://niw.ctjpmb.com

[J08] 提取年月日与星期
来源：http://iyw.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nlg.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pse.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ude.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tku.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ipc.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nfw.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mjk.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://act.cheryme.top

[J09] 时区处理
来源：http://bac.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://daw.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hbp.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tra.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aka.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dvb.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nue.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qip.yuanzhike.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jgg.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://jxd.yfazqb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://uqg.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bqz.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iwh.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vze.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pgb.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://woa.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ewq.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://isy.jqgfzy.top

================================================================================
来源：http://dkr.chenlongwang.top

K. JSON 与序列化
来源：http://gso.shangyingyoupin.top

================================================================================
来源：http://kyj.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://vnx.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rkc.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dtz.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://jwy.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://kgk.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lfx.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://wwe.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://ylj.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wff.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://ycx.yj20258.top

Py:   json.loads(s)
来源：http://bpz.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://spl.hywenlv.cn

JS:   JSON.parse(s)
来源：http://rnp.316326.xyz

TS:   JSON.parse(s)
来源：http://pno.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mum.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://hgj.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://lvm.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dgi.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://jtx.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wtj.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yaq.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dqy.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://jvo.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wcm.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tve.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kcv.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qbl.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://dbz.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://plp.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qgq.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sjv.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://poj.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zwr.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://deo.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qlq.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://svr.sysykeji.top

[K05] 深拷贝对象
来源：http://dva.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://mec.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://dti.yfazqb.com

JS:   structuredClone(obj)
来源：http://dcj.ybcxt.top

TS:   structuredClone(obj)
来源：http://bgo.daxiang520.top


<!-- 参考信息 -->