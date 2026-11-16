代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://gxs.ivvv.top

Ruby: obj.instance_variables
来源：http://xan.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://szv.fehbvm.com

================================================================================
来源：http://zgl.ydjk.org.cn

H. 异常与错误处理
来源：http://lcu.shanyushiyangtech.top

================================================================================
来源：http://alp.iojbl.cn

[H01] try / catch 基础
来源：http://ito.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ahb.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pgo.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kfp.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ezr.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ype.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://deg.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://izf.daria6918.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oqn.ybcxt.top

[H02] finally / ensure 收尾
来源：http://gkz.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://fvg.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ary.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ztl.shangyingyoupin.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fox.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uly.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ody.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qce.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ckd.kuanghao11.cn

[H03] 主动抛出异常
来源：http://fwh.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://dyu.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ufl.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://ind.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://wyr.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xdf.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fmb.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dxy.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://spo.smart0.xyz

[H04] 自定义异常类型
来源：http://eln.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://jcn.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://san.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://cyo.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://nmy.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://idf.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vky.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://ryw.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://kqo.kuanghao11.cn

[H05] 捕获特定类型
来源：http://sgo.yj20258.top

Py:   except ValueError as e:
来源：http://bxf.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://riw.ctjpmb.com

JS:   if (e instanceof TypeError) {}
来源：http://bnf.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://ost.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://eij.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oph.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://onb.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kha.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://khn.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://oin.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://yax.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://jay.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xiz.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iyy.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ojl.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://vnk.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://dln.yj202588.top

[H07] 断言
来源：http://bft.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://utq.mhx1999.top

PHP:  assert($x > 0);
来源：http://bmg.shuidangran.top

JS:   console.assert(x > 0);
来源：http://bjf.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://lax.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://dda.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kko.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://tzm.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://oqr.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://gwx.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://mov.wangdashe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://his.zhengqikj.top

JS:   e.message;  e.stack
来源：http://atz.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zjj.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nwc.ehwqpu.com

Go:   err.Error()
来源：http://jtg.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://gnp.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://nvu.yuxming.cn

[H09] 带错误码的异常
来源：http://zps.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://imw.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://brh.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eym.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zuy.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dhn.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://atc.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://yyg.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hbb.svipenyu.cn

[H10] 资源自动释放
来源：http://dyr.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://elf.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pko.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ybj.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ifj.daria6918.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ugg.zdbjq.cn

Go:   defer f.Close()
来源：http://diu.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jfu.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://soj.guannengcc.top

================================================================================
来源：http://nsb.haohaochexian.top

I. 正则表达式
来源：http://myg.fanxiaobao.xyz

================================================================================
来源：http://cxq.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://rcm.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wwe.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://glo.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://yss.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://wxg.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vue.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqv.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://pgu.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://per.zhengqikj.top

[I02] 提取所有匹配
来源：http://scf.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://kgr.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aql.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yhf.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://xcg.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cpj.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://imd.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://pgy.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://caq.svipenyu.cn

[I03] 提取捕获分组
来源：http://rbj.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rud.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lxe.chenjidiqi.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gef.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lze.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cid.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ija.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xtc.sufxvd.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://agy.smart0.xyz

[I04] 正则替换
来源：http://yvx.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qyb.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uby.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://ihq.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vob.jlsjyb.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ubz.shanyushiyangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vhs.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kwk.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://awm.birdmap.top

[I05] 按正则拆分
来源：http://bxh.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xaf.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rxz.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://yks.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://knw.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://zue.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dup.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://eqv.tarul.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lvo.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ooz.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://efy.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iwp.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lig.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csb.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hpn.sxryk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sgb.yvedp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ipd.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qje.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://xpe.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wek.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://erl.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vpu.fzhhl.top

TS:   /error/gim
来源：http://rwe.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://abf.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bhq.yangfankeji.com

Ruby: s.scan(/error/i)
来源：http://kha.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://scb.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://wuf.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mgk.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wcf.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mzd.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ren.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bjb.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wwl.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ztl.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xfu.shanyushiyangkeji.top

================================================================================
来源：http://gmz.vehdjk.com

J. 日期与时间
来源：http://npw.fehbvm.com

================================================================================
来源：http://inr.andypj.xyz

[J01] 获取当前时间
来源：http://jol.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rwd.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ksq.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://mol.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://jro.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yvk.wangdashe.top

Go:   time.Now()
来源：http://bil.snrcjt.cn

Ruby: Time.now
来源：http://zab.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://evu.fktsv.cn

[J02] 格式化输出
来源：http://agf.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uke.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jbb.zdqjudy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://msz.guannengcc.top

TS:   d.toISOString()
来源：http://rnf.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://exz.jinyuanbaomall.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sip.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jld.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zbx.52xcode.cn

[J03] 字符串解析为日期
来源：http://zna.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zey.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jke.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://fwp.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://qek.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://nko.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://imy.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://nnd.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tpo.pycfn.com

[J04] 时间戳与日期互转
来源：http://ify.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qgg.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kdr.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qfd.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cml.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zaz.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bip.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wbe.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yem.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://bmu.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://elr.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xiv.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qzr.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://psx.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://fhp.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sbg.shanyushiyangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://xjb.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://wnm.c1oappe.top

[J06] 计算两时间之差
来源：http://dcd.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://vyb.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://dmd.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://goh.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gzu.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qpd.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://ijs.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://aij.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://xkm.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://imo.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://grl.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://via.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://dnf.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://zep.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jhx.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wts.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://hqg.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://mjy.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://syt.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gsq.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qkt.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xjc.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mjr.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cic.meibo888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hig.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://apa.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fdp.daxiang520.top

[J09] 时区处理
来源：http://vgo.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fkr.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kww.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqr.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hyb.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://onm.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wrh.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hty.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ncm.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://sir.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://idp.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tnw.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wfj.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dwc.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zmi.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xhr.havefunace.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ych.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yrs.shanyushiyangtech.top

================================================================================
来源：http://ylg.vqdsnc.cn

K. JSON 与序列化
来源：http://xjz.ppjwa.cn

================================================================================
来源：http://lki.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://ylh.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ufe.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hmm.yj202588.top

JS:   JSON.stringify(obj)
来源：http://mwi.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://gcj.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://usg.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://twc.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://dkt.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jci.epnwcf.com

[K02] JSON 字符串转对象
来源：http://ict.hnqzz.top

Py:   json.loads(s)
来源：http://cqt.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bor.gotoacloud.top

JS:   JSON.parse(s)
来源：http://kqd.aizwys.cn

TS:   JSON.parse(s)
来源：http://euz.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wao.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://hrc.fktsv.cn

Ruby: JSON.parse(s)
来源：http://aqo.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://opf.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://mle.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://drz.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lpo.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ezr.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bav.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wew.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wbm.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://gpa.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gjz.52xcode.cn

[K04] 读取 JSON 文件
来源：http://jpt.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zfv.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ihp.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ttb.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kht.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jyk.hywenlv.cn


<!-- 参考信息 -->