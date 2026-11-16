代发 wailian999

PHP:  get_object_vars($obj);
来源：http://uwv.vehdjk.com

JS:   Object.entries(obj)
来源：http://tug.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://unz.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://owi.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fzk.yj20258888.top

Ruby: obj.instance_variables
来源：http://ndm.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://pmr.jyoumei.cn

================================================================================
来源：http://reg.yj202588.top

H. 异常与错误处理
来源：http://zua.zhiwuduotai.top

================================================================================
来源：http://nbx.andypj.xyz

[H01] try / catch 基础
来源：http://mas.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ucp.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ixa.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://coz.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fze.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vtg.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xnz.birdmap.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hej.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zgd.sysykeji.top

[H02] finally / ensure 收尾
来源：http://ave.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://rzs.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xhu.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fmk.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ouh.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bvq.vqdsnc.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qyq.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cej.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bbe.dianchejie.cn

[H03] 主动抛出异常
来源：http://hyn.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://onz.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mid.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://pgs.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://xny.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xtx.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mbd.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ztf.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dqk.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://qsn.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://ull.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qva.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://ebo.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://ksj.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://rtw.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fjh.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://rmw.aizwys.cn

C#:   class MyException : Exception {}
来源：http://fsr.fanxiaobao.xyz

[H05] 捕获特定类型
来源：http://svk.yj20258.top

Py:   except ValueError as e:
来源：http://eca.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zgr.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://erx.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://oii.cheryme.top

Java: catch (IOException | SQLException e) {}
来源：http://suw.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ffn.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://qnv.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fjl.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://zxx.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://tam.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://hwr.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://naa.shuidangran.top

TS:   obj?.a?.b;  d ?? default
来源：http://vha.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qlh.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://opb.hysaishi.cn

Ruby: d&.dig(:a, :b)
来源：http://kpk.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://otd.yonumen.top

[H07] 断言
来源：http://yme.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://kmh.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://qbh.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://mnn.ybcxt.top

TS:   console.assert(x > 0);
来源：http://kqo.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://tay.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pgx.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://erj.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://hgj.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://bup.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://qkt.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zbw.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://nmr.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xqc.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ehe.jinyuanbaomall.cn

Go:   err.Error()
来源：http://emh.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://rqc.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://sws.bbcook.cn

[H09] 带错误码的异常
来源：http://hia.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bzs.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://frs.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dmr.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qdv.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jnw.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xct.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://oqt.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tux.gzhubu.top

[H10] 资源自动释放
来源：http://vnj.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://bjj.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aqf.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ehu.tianlin.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aco.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gab.pengpengdd.cyou

Go:   defer f.Close()
来源：http://nqr.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://twh.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://khj.pycfn.com

================================================================================
来源：http://jkw.jqgfzy.top

I. 正则表达式
来源：http://zfa.hfpthk.cn

================================================================================
来源：http://omf.zycfv.cn

[I01] 判断是否匹配
来源：http://rtz.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rua.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bes.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://dwm.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://jqr.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zui.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jpv.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://yhm.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hmn.kuanghao11.cn

[I02] 提取所有匹配
来源：http://lhb.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://bgh.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://scm.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bhr.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://anl.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pgx.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kno.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://fye.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fqu.yj20258888.top

[I03] 提取捕获分组
来源：http://txr.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://olm.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sgw.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wfy.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rht.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zmb.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mqg.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nqi.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vvy.jiagoushi.top

[I04] 正则替换
来源：http://lzz.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://mos.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jza.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cgf.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lun.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://qah.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hym.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://azu.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nrj.zhiwuduotai.top

[I05] 按正则拆分
来源：http://kgj.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bwb.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cge.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://ohk.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://kek.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://bhx.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yoj.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://biz.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ftm.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sye.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uvm.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pzs.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gmj.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fsg.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kng.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://txc.tanke756.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vna.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uvd.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://fcz.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://icz.nwbrower.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cgs.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uhg.kuanghao11.cn

TS:   /error/gim
来源：http://xil.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bti.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vyb.tarul.cn

Ruby: s.scan(/error/i)
来源：http://ezl.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lwk.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://nei.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iny.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://enh.hcnkem.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xuo.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://odj.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ihx.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://usl.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jvo.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qfg.yongpay.top

================================================================================
来源：http://sol.xuanzx.com

J. 日期与时间
来源：http://fji.nanxuanxn.top

================================================================================
来源：http://rrv.haohaochexian.top

[J01] 获取当前时间
来源：http://yte.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://nxi.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lhl.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://efu.tarul.cn

TS:   new Date();  Date.now()
来源：http://pjl.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://dak.quarkkingdee.top

Go:   time.Now()
来源：http://hmh.shzxlz.cn

Ruby: Time.now
来源：http://nrp.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bux.kuanghao11.cn

[J02] 格式化输出
来源：http://hsu.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wyo.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rki.bbcook.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://twd.zhongyouzk.top

TS:   d.toISOString()
来源：http://sys.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ppa.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://joh.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ejl.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ubq.nwbrower.top

[J03] 字符串解析为日期
来源：http://hut.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hdx.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://upl.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://rxa.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://uem.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://wgq.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://skv.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://amb.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gnn.xziqi.cn

[J04] 时间戳与日期互转
来源：http://fvu.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ioa.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pqw.wangshuangyany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://raz.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://glq.shangyingyoupin.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pzw.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ddf.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ihh.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://enq.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://tlh.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://rsf.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xwn.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iaq.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lka.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://ens.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lub.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://fzx.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://ogl.hfpthk.cn

[J06] 计算两时间之差
来源：http://fho.cheryme.top

Py:   (end - start).total_seconds()
来源：http://zyb.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://pnt.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mtk.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cei.tian-w.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kjz.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://umj.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://vhy.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://lje.9152youxi.cn

[J07] 比较两个日期
来源：http://ata.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ovw.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://khk.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nuh.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://rrn.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bbt.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ftr.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://jsp.xinyue.icu

C#:   d1 < d2;  d1 == d2
来源：http://eko.havefunace.top

[J08] 提取年月日与星期
来源：http://yei.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ner.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nux.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qdg.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vxr.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vrs.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nbj.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ure.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zrw.316326.xyz

[J09] 时区处理
来源：http://bro.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fot.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qkn.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xan.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcs.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lju.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tyv.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://qrp.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://max.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://ivm.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://and.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cxn.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://frd.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ody.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vao.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zxs.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bmp.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eds.yueranfly.top

================================================================================
来源：http://bqz.bjfxy.top

K. JSON 与序列化
来源：http://sre.yj202588.top

================================================================================
来源：http://mcy.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://afk.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aal.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xnw.pycfn.com

JS:   JSON.stringify(obj)
来源：http://nkx.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://vzs.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ufa.hesvh.cn

Go:   json.Marshal(obj)
来源：http://jwx.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://arm.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lus.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://qvq.xuanzx.com

Py:   json.loads(s)
来源：http://iyj.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mgm.jiagoushi.top

JS:   JSON.parse(s)
来源：http://nxg.guannengcc.top

TS:   JSON.parse(s)
来源：http://xlk.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://reg.vqdsnc.cn

Go:   json.Unmarshal(data, &v)
来源：http://jep.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://kvb.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sjm.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://kqh.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uvx.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hae.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uzk.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zqz.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tqe.yvedp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cml.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://qzm.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nxi.redwolf501.top

[K04] 读取 JSON 文件
来源：http://jfu.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zqx.ydjk.org.cn


<!-- 参考信息 -->