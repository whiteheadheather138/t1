代发 wailian999

PHP:  get_object_vars($obj);
来源：http://fyg.dashuyun.cn

JS:   Object.entries(obj)
来源：http://wfs.ivvv.top

TS:   Object.entries(obj)
来源：http://bvt.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ebx.fktsv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wzj.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://lrq.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://sgm.daxiang520.top

================================================================================
来源：http://gkd.aizwys.cn

H. 异常与错误处理
来源：http://moj.shangyingyoupin.top

================================================================================
来源：http://igd.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://ddy.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nfw.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fvg.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ttx.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fqa.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gad.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hcq.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ltl.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cjk.nwbrower.top

[H02] finally / ensure 收尾
来源：http://pkq.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://bsx.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zkv.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vgk.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://myq.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://tlc.hysaishi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ijl.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cvm.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qjt.pycfn.com

[H03] 主动抛出异常
来源：http://boq.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://yag.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bxu.xziqi.cn

JS:   throw new Error("错误信息");
来源：http://cca.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://wsq.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gvy.zhixingplan.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kwi.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fjh.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://gzw.yonumen.top

[H04] 自定义异常类型
来源：http://nzg.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://bwx.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://vee.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://dls.yueranfly.top

TS:   class MyError extends Error {}
来源：http://tvs.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://qep.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kgw.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://ykz.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://crh.jyoumei.cn

[H05] 捕获特定类型
来源：http://ihi.jlsjyb.cn

Py:   except ValueError as e:
来源：http://htu.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qqm.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://suf.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://zcb.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://zhs.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kmb.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://eai.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lkq.xziqi.cn

[H06] 可选值 / 空值安全访问
来源：http://uic.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://qvg.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://nxf.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://frj.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qbv.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://emg.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cbm.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://qca.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://cho.ydjk.org.cn

[H07] 断言
来源：http://xmg.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://ouy.yj202588.top

PHP:  assert($x > 0);
来源：http://ebn.hfpthk.cn

JS:   console.assert(x > 0);
来源：http://mdt.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://djf.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://axs.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://asw.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://lss.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://fsu.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://qrz.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://pji.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yyu.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://gnr.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://iul.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zcx.ydjk.org.cn

Go:   err.Error()
来源：http://guy.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://tut.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://avz.zhengqikj.top

[H09] 带错误码的异常
来源：http://dec.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wpo.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://erp.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qzf.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ntt.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vbg.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mnz.ybcxt.top

Ruby: raise MyError.new("fail", 500)
来源：http://kyx.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pmd.yongpay.top

[H10] 资源自动释放
来源：http://bdi.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://vih.xingfuxueyuan.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://upv.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ycy.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gvj.zhaomingkeji.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nnp.wangdashe.top

Go:   defer f.Close()
来源：http://svt.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fss.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://moy.cheryme.top

================================================================================
来源：http://lbz.9152youxi.cn

I. 正则表达式
来源：http://wyh.tanke756.top

================================================================================
来源：http://pjo.meibo888.top

[I01] 判断是否匹配
来源：http://uvl.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qba.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://bat.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://wqj.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://iwe.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ppj.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ldi.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://lkx.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://anc.fzhhl.top

[I02] 提取所有匹配
来源：http://kpa.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://ukz.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dos.hnqzz.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vui.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://xko.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://szb.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vra.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://kme.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jws.jyoumei.cn

[I03] 提取捕获分组
来源：http://qma.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gqi.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lcy.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rgf.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rtn.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kev.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dvy.wangshuangyany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lgi.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://azm.hcnkem.com

[I04] 正则替换
来源：http://jun.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kkw.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dew.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://crg.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://rbe.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://aln.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hej.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://egr.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ass.0kj1m.cn

[I05] 按正则拆分
来源：http://uke.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zjy.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://flp.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://kol.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://dzu.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://fjq.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mho.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hee.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dbz.52xcode.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zkx.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iga.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sav.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uop.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ilb.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yuw.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fum.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kbj.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fut.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://pna.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hbq.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nfa.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://arm.9152youxi.cn

TS:   /error/gim
来源：http://oop.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://map.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cyr.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://tvv.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uvq.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://rej.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ieo.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jaq.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lmc.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zue.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://wdr.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lib.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kga.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eeq.vqdsnc.cn

================================================================================
来源：http://fue.jinghuilouyu.cn

J. 日期与时间
来源：http://qht.xinyue.icu

================================================================================
来源：http://awi.zhoulong.xyz

[J01] 获取当前时间
来源：http://pqf.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tmw.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mum.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://wnr.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://ood.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://slt.dianchejie.cn

Go:   time.Now()
来源：http://mmu.pengpengdd.cyou

Ruby: Time.now
来源：http://tmt.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kae.epnwcf.com

[J02] 格式化输出
来源：http://gms.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfm.shzxlz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ukj.dashuyun.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://obz.yuxming.cn

TS:   d.toISOString()
来源：http://tlg.tanke756.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oug.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mvv.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://etc.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hja.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://gvy.redwolf501.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rfk.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kov.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://zrv.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://rnn.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://mcy.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gnu.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://mgq.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ahg.fehbvm.com

[J04] 时间戳与日期互转
来源：http://jrg.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lmy.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dbd.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pdc.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jct.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://skc.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xeh.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dkc.mhx1999.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dpx.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://itn.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://alp.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://enz.svipenyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://elg.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kge.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://fzr.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wgr.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://idn.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://prd.yuxming.cn

[J06] 计算两时间之差
来源：http://jtt.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://ruu.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://vzh.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vmx.xziqi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lbq.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://zhr.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://rfz.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://ule.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://spi.cqqwz.cn

[J07] 比较两个日期
来源：http://tup.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://txx.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cfr.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://gkg.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://voc.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xbq.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://una.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://dax.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://jbb.xuanzx.com

[J08] 提取年月日与星期
来源：http://pua.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qwg.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zqj.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://swo.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oqj.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hgl.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cbg.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zcw.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://foh.gzhubu.top

[J09] 时区处理
来源：http://snu.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rum.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wzr.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wtz.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zqs.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qdu.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hvw.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://abk.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mua.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://xcp.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tbu.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ayn.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yfr.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vxj.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jht.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://awg.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://org.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wrc.shuidangran.top

================================================================================
来源：http://xea.zhijiandao.cn

K. JSON 与序列化
来源：http://mag.andypj.xyz

================================================================================
来源：http://zur.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://lwp.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://syx.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://txk.havefunace.top

JS:   JSON.stringify(obj)
来源：http://uum.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://fyr.havefunace.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zoz.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://cln.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://vjr.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ksg.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://jlg.ybcxt.top

Py:   json.loads(s)
来源：http://snb.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sym.ctjpmb.com

JS:   JSON.parse(s)
来源：http://vdu.haohaochexian.top

TS:   JSON.parse(s)
来源：http://eov.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xub.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://kuq.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://kfu.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dmm.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://tzr.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ggo.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hps.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qkn.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ynv.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nvm.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://crk.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://lnu.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yto.yuxming.cn

[K04] 读取 JSON 文件
来源：http://lxs.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yot.jyoumei.cn


<!-- 参考信息 -->