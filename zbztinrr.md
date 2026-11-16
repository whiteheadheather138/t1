代发 wailian999

PHP:  get_object_vars($obj);
来源：http://xjq.fktsv.cn

JS:   Object.entries(obj)
来源：http://cyv.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://yix.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://smv.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://esa.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://asj.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://csl.yangfankeji.com

================================================================================
来源：http://zii.zhijiandao.cn

H. 异常与错误处理
来源：http://dpr.sxryk.cn

================================================================================
来源：http://xhn.havefunace.top

[H01] try / catch 基础
来源：http://nma.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mnm.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zhj.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://smr.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lhs.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ats.aizwys.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oas.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dfn.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://klk.cucudq.cn

[H02] finally / ensure 收尾
来源：http://oig.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uij.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yoo.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tqn.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://dpg.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://krl.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://svc.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tbs.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sez.tarul.cn

[H03] 主动抛出异常
来源：http://mwu.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://qko.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hqa.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://zrd.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://gbf.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lap.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://umj.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cyc.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://boq.hesvh.cn

[H04] 自定义异常类型
来源：http://fri.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://eka.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://nlo.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://dvm.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://nlc.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://cgi.hfpthk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dpq.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://sbe.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://cru.hammf.cn

[H05] 捕获特定类型
来源：http://gtz.ehwqpu.com

Py:   except ValueError as e:
来源：http://rbq.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dtm.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://ttg.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://stg.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://loj.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rae.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://yhk.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xlp.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://yvk.cucudq.cn

Py:   value = d.get("k") or default
来源：http://ntf.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://whn.zhiwuduotai.top

JS:   obj?.a?.b;  d ?? default
来源：http://apz.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bep.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rcx.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ccz.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://dvo.hysaishi.cn

C#:   obj?.A?.B ?? default
来源：http://kfn.ybcxt.top

[H07] 断言
来源：http://ovp.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://fyo.hysaishi.cn

PHP:  assert($x > 0);
来源：http://fvo.vehdjk.com

JS:   console.assert(x > 0);
来源：http://wdr.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://uqb.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://hmi.xinyue.icu

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qhx.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://auu.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://mpf.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://jmr.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://poe.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sdz.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://dpc.gogol.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rog.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://pwq.cheryme.top

Go:   err.Error()
来源：http://kgh.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://emw.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://uyb.meibo888.top

[H09] 带错误码的异常
来源：http://yqd.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://slp.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rjo.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://znf.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mws.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dzf.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qhd.hongshengwenyu.top

Ruby: raise MyError.new("fail", 500)
来源：http://vtx.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rxb.havefunace.top

[H10] 资源自动释放
来源：http://jbr.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bab.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tpw.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hnu.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kmt.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uwp.zhoulong.xyz

Go:   defer f.Close()
来源：http://scp.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nla.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qod.zdbjq.cn

================================================================================
来源：http://jbu.sufxvd.cn

I. 正则表达式
来源：http://pml.zhengqikj.top

================================================================================
来源：http://cqk.gogol.net.cn

[I01] 判断是否匹配
来源：http://xvs.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tyq.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rev.daria6918.cn

JS:   /\d+/.test(s)
来源：http://czq.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://vcd.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gdq.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sop.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://szc.shzxlz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://izj.uphjek.com

[I02] 提取所有匹配
来源：http://uim.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://mip.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iym.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ilz.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://vyz.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dwi.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jls.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://wvw.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://byw.zycfv.cn

[I03] 提取捕获分组
来源：http://tsn.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://arl.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jfo.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://igc.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ilv.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mmn.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wtb.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yui.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nbv.sjlbkw.cn

[I04] 正则替换
来源：http://zsi.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fpb.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vtq.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kye.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zsn.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://kwg.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qtk.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ila.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kpb.ctjpmb.com

[I05] 按正则拆分
来源：http://tvf.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nov.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uze.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://rjc.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://hau.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://ucp.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tri.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://sto.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qlm.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nto.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bgm.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hrr.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bdo.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mba.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lmz.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ops.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jwc.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lsd.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://lqr.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jrs.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fwb.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ezr.jinqigufen.top

TS:   /error/gim
来源：http://zdc.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bzm.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ueg.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://wpz.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fxv.epnwcf.com

[I08] 贪婪与非贪婪匹配
来源：http://qom.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gcq.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vyy.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://twu.yangfankeji.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqo.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kxr.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jjd.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wxg.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uss.chenzaomai.com

================================================================================
来源：http://niw.fanxiaobao.xyz

J. 日期与时间
来源：http://chy.zhixingplan.top

================================================================================
来源：http://mta.jlsjyb.cn

[J01] 获取当前时间
来源：http://bli.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://etq.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qvl.guannengcc.top

JS:   new Date();  Date.now()
来源：http://avi.zycfv.cn

TS:   new Date();  Date.now()
来源：http://cif.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tbl.jinyuanbaomall.cn

Go:   time.Now()
来源：http://vog.yj202588.top

Ruby: Time.now
来源：http://qgv.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zeo.sweek.top

[J02] 格式化输出
来源：http://rup.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ybp.shuidangran.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wgw.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fdt.zhiwuduotai.top

TS:   d.toISOString()
来源：http://idc.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://phx.ehwqpu.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bwe.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ugk.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wmd.xuanzx.com

[J03] 字符串解析为日期
来源：http://fuy.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bac.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qwd.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://jcd.xuetiantiany.cn

TS:   new Date("2024-01-02")
来源：http://eqw.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://obz.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cxh.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://lom.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pqg.fktsv.cn

[J04] 时间戳与日期互转
来源：http://guz.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://onp.jqgfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://thx.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qei.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fuf.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://scn.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wys.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mlz.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vlu.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://qiw.yonumen.top

Py:   now + timedelta(days=7)
来源：http://dji.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://diu.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fsv.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ztz.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://duq.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ejd.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://ake.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ldq.sjlbkw.cn

[J06] 计算两时间之差
来源：http://mch.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://iuo.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://kwn.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ffh.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rmf.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://lbp.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://fcq.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://osa.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://thm.cashguo.top

[J07] 比较两个日期
来源：http://sbq.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://ygk.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tyv.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://dzo.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://hvw.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nvr.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gsp.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://syv.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://dqb.zhixingplan.top

[J08] 提取年月日与星期
来源：http://jmr.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iye.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://osh.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ktx.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qxd.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gdm.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qtz.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rvl.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cby.zhengqikj.top

[J09] 时区处理
来源：http://tge.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ttp.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ilf.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kdf.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pey.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fds.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wox.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://byf.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ble.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://dld.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ysx.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bop.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jyu.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://prt.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uyo.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pew.andypj.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hvz.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jxy.ivvv.top

================================================================================
来源：http://zpf.mhx1999.top

K. JSON 与序列化
来源：http://kgu.guowangkeji.top

================================================================================
来源：http://day.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://xwi.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gma.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://drv.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://qry.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://rdb.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uyb.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://fis.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://vqd.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://pbm.hammf.cn

[K02] JSON 字符串转对象
来源：http://bcx.0kj1m.cn

Py:   json.loads(s)
来源：http://rnm.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://off.sweek.top

JS:   JSON.parse(s)
来源：http://slz.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://bfh.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wpc.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://tsr.xinyue.icu

Ruby: JSON.parse(s)
来源：http://urz.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://acj.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://dco.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://paf.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wve.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fkj.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lpm.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dqh.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fka.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://vje.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fzn.ivvv.top

[K04] 读取 JSON 文件
来源：http://eip.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://abi.snrcjt.cn


<!-- 参考信息 -->