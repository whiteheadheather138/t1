代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kvp.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://myu.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://mxn.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mfe.hywenlv.cn

Ruby: Color = %i[red green].freeze
来源：http://fiy.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uxv.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://fvy.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hnc.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://pxq.jinqigufen.top

JS:   Object.entries(obj)
来源：http://aad.chenlongwang.top

TS:   Object.entries(obj)
来源：http://jsu.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bzv.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lfn.guowangkeji.top

Ruby: obj.instance_variables
来源：http://rxh.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://gze.gaohongyu789.top

================================================================================
来源：http://ore.ivvv.top

H. 异常与错误处理
来源：http://ief.jinqigfzy.top

================================================================================
来源：http://xlz.tianlin.xyz

[H01] try / catch 基础
来源：http://gtf.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rsp.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://phw.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://muz.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zjt.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uno.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://etg.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dxp.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qle.xylfe.cn

[H02] finally / ensure 收尾
来源：http://hew.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://nuw.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qyc.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://shc.shangyingyoupin.top

TS:   try { f(); } finally { cleanup(); }
来源：http://slf.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://anu.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xru.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wuy.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://squ.aizwys.cn

[H03] 主动抛出异常
来源：http://wei.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://cdb.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://doe.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://xnd.yongpay.top

TS:   throw new Error("错误信息");
来源：http://qcl.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://kmo.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kov.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://amc.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://otr.316326.xyz

[H04] 自定义异常类型
来源：http://lff.yongpay.top

Py:   class MyError(Exception): pass
来源：http://fza.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://moe.iojbl.cn

JS:   class MyError extends Error {}
来源：http://wgi.redwolf501.top

TS:   class MyError extends Error {}
来源：http://isj.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://jbl.chenjidiqi.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lcy.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://ije.cashguo.top

C#:   class MyException : Exception {}
来源：http://bpf.vehdjk.com

[H05] 捕获特定类型
来源：http://jms.chenlongwang.top

Py:   except ValueError as e:
来源：http://csu.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fts.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://xyp.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://cxt.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://qcw.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qaf.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://mdm.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wwc.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://yyb.fzhhl.top

Py:   value = d.get("k") or default
来源：http://ufi.kuanghao11.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hsi.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://yet.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://oqh.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blp.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bfd.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://als.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://ezc.yuxming.cn

[H07] 断言
来源：http://ozd.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://awk.hesvh.cn

PHP:  assert($x > 0);
来源：http://bci.fengsongda.top

JS:   console.assert(x > 0);
来源：http://myx.cheryme.top

TS:   console.assert(x > 0);
来源：http://fxm.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://nwz.yvedp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://arz.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://fmo.yanxiufei.cn

C#:   Debug.Assert(x > 0);
来源：http://cuu.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://hbw.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://lvh.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pgy.tanke756.top

JS:   e.message;  e.stack
来源：http://vlm.shuidangran.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xya.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://buh.jinyuanbaomall.cn

Go:   err.Error()
来源：http://cgu.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://eri.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://aur.zdbjq.cn

[H09] 带错误码的异常
来源：http://kjf.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rjf.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://oac.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fhh.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://erp.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ggs.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dzh.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://saa.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mek.iojbl.cn

[H10] 资源自动释放
来源：http://spn.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aid.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jgl.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kru.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fmf.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jvu.bbcook.cn

Go:   defer f.Close()
来源：http://vit.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://piu.zdbjq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cdp.zhengqikj.top

================================================================================
来源：http://jaj.xuanzx.com

I. 正则表达式
来源：http://hlm.ydzc1.top

================================================================================
来源：http://eow.jlsjyb.cn

[I01] 判断是否匹配
来源：http://njs.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jdw.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iaf.daxiang520.top

JS:   /\d+/.test(s)
来源：http://qpw.yj20258.top

TS:   /\d+/.test(s)
来源：http://bom.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jck.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://plo.xuanzx.com

Ruby: s.match?(/\d+/)
来源：http://gaa.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://haw.daxiang520.top

[I02] 提取所有匹配
来源：http://cni.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://lno.pengpengdd.cyou

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vup.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kry.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://yzv.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dlk.sweek.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://clq.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://igk.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vwm.sweek.top

[I03] 提取捕获分组
来源：http://shm.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jfs.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://psq.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://edc.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jqs.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fkx.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tuo.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cqe.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dnj.nanxuanxn.top

[I04] 正则替换
来源：http://fzv.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vpr.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gwx.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://alc.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qpd.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://ril.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oiy.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://diw.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lsx.bbcook.cn

[I05] 按正则拆分
来源：http://jzl.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vsi.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://exk.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://tdz.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://cod.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://qzi.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wtk.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wsh.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://esa.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://avs.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fum.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hou.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dpe.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msy.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yws.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://axp.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://akg.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oze.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://zew.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://scf.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wtj.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gbz.redwolf501.top

TS:   /error/gim
来源：http://jrr.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wwa.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mqy.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://omr.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vgj.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://ofu.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://law.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://liv.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tnj.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vrp.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://dwg.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jde.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lrz.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jul.vqdsnc.cn

================================================================================
来源：http://esz.pengpengdd.cyou

J. 日期与时间
来源：http://mlh.jinqigufen.top

================================================================================
来源：http://pgo.yj20258.top

[J01] 获取当前时间
来源：http://jbe.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zey.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vlo.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://bbt.daria6918.cn

TS:   new Date();  Date.now()
来源：http://olv.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yrh.svipenyu.cn

Go:   time.Now()
来源：http://rvt.guannengcc.top

Ruby: Time.now
来源：http://wbv.jinqigfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hvk.tarul.cn

[J02] 格式化输出
来源：http://gkc.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wzm.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://flh.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://esh.yj20258888.top

TS:   d.toISOString()
来源：http://gnz.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qcr.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gjq.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kvg.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gum.yueranfly.top

[J03] 字符串解析为日期
来源：http://oki.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qtd.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://asb.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://kff.feifeiyinyue.top

TS:   new Date("2024-01-02")
来源：http://kxl.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://ajv.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vjb.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://ghc.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zjg.vehdjk.com

[J04] 时间戳与日期互转
来源：http://uww.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vvh.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://scg.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zch.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ogg.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ovo.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hwn.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jrh.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://imr.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://qpq.cashguo.top

Py:   now + timedelta(days=7)
来源：http://yec.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lmp.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://koh.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fgr.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://jvg.guannengcc.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tvu.hcnkem.com

Ruby: Time.now + 7 * 86400
来源：http://bss.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://udu.birdmap.top

[J06] 计算两时间之差
来源：http://cyl.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://nsm.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://itd.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wsw.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rlv.guowangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://sbc.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://lns.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://fsy.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://vlz.svipenyu.cn

[J07] 比较两个日期
来源：http://xkd.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://smw.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bbv.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://owr.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zwj.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vkx.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://idu.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xmk.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://bfv.tanke756.top

[J08] 提取年月日与星期
来源：http://ykv.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tvu.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ckf.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wly.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://skb.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ffp.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://idu.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fym.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://was.jlsjyb.cn

[J09] 时区处理
来源：http://lyh.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zqz.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ocn.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ldr.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rjm.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yhs.cashguo.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vdv.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qil.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ktq.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://usp.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://reh.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xho.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hfd.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vje.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wsg.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mvk.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cgi.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tqz.chenzaomai.com

================================================================================
来源：http://lke.c1oappe.top

K. JSON 与序列化
来源：http://fhx.yueranfly.top

================================================================================
来源：http://tzm.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://bqy.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ysm.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nhm.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://fap.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://vzv.316326.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bht.zycfv.cn

Go:   json.Marshal(obj)
来源：http://jfy.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bbs.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://uxk.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://acc.shangyingyoupin.top

Py:   json.loads(s)
来源：http://irh.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rgg.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://sps.wangdashe.top

TS:   JSON.parse(s)
来源：http://gav.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://enq.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://kqn.uphjek.com

Ruby: JSON.parse(s)
来源：http://qhb.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hrg.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://ncr.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lru.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dws.shangyingyoupin.top


<!-- 参考信息 -->