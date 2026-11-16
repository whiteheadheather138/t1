代发 wailian999

C#:   record User(string Name, int Age);
来源：http://fxl.havefunace.top

[G15] 枚举
来源：http://qsz.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://smu.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://src.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ksw.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://spp.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://lga.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rxl.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://zol.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://whl.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://ufb.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://msl.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://zmr.guannengcc.top

JS:   Object.entries(obj)
来源：http://lch.aizwys.cn

TS:   Object.entries(obj)
来源：http://ehm.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kif.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uil.hammf.cn

Ruby: obj.instance_variables
来源：http://ffy.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://jdp.fehbvm.com

================================================================================
来源：http://pzj.guannengcc.top

H. 异常与错误处理
来源：http://vqw.chenlongwang.top

================================================================================
来源：http://qzz.uphjek.com

[H01] try / catch 基础
来源：http://xhf.dashuyun.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zox.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dxd.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vju.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ofg.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jmq.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eij.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yxi.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ivj.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://oyw.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xfk.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ees.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dne.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://alp.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://htj.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zmh.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hzi.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gxj.dashuyun.cn

[H03] 主动抛出异常
来源：http://okj.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://cdu.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kfr.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://etf.tanke756.top

TS:   throw new Error("错误信息");
来源：http://cwf.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://idd.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bgh.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://opp.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://bkf.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://bhi.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://yks.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fdx.smart0.xyz

JS:   class MyError extends Error {}
来源：http://dip.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://lhd.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://oef.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ayz.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://kpe.wangdashe.top

C#:   class MyException : Exception {}
来源：http://egp.zhongyouzk.top

[H05] 捕获特定类型
来源：http://yqw.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://uwk.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ukl.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://tvb.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://hzh.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://lsl.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ebq.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://kqo.hysaishi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kfi.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://iiz.hnqzz.top

Py:   value = d.get("k") or default
来源：http://rbx.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ift.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gay.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://ioo.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mdf.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ecz.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://xcn.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://nzt.zdqjudy.top

[H07] 断言
来源：http://pee.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://dlq.shzxlz.cn

PHP:  assert($x > 0);
来源：http://fmq.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://bwg.xinyue.icu

TS:   console.assert(x > 0);
来源：http://kfc.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://fzg.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zji.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://kcj.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://axl.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://fyg.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ody.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cli.9152youxi.cn

JS:   e.message;  e.stack
来源：http://cfy.shuidangran.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ece.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uyy.fehbvm.com

Go:   err.Error()
来源：http://kzk.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://fds.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://xss.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://ekq.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://swz.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://obt.cashguo.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://suc.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nue.ywan-chungtsiang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wsm.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ccu.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://mvm.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://acg.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://zpg.fktsv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tps.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jjo.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fmc.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ogq.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rjb.9152youxi.cn

Go:   defer f.Close()
来源：http://lqr.sufxvd.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xce.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hea.tianlin.xyz

================================================================================
来源：http://bby.pycfn.com

I. 正则表达式
来源：http://czm.dianchejie.cn

================================================================================
来源：http://ffr.c1oappe.top

[I01] 判断是否匹配
来源：http://vud.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rnx.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fcm.cucudq.cn

JS:   /\d+/.test(s)
来源：http://ksm.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://qtf.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lvk.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pnk.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://rjv.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mgu.yuanzhike.top

[I02] 提取所有匹配
来源：http://bif.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://egx.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zun.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yrl.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://ugg.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gtf.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cmb.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://mix.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rbm.uphjek.com

[I03] 提取捕获分组
来源：http://tdd.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mof.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ycr.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yhn.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lxc.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://olv.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ovz.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://olf.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kaz.nwbrower.top

[I04] 正则替换
来源：http://ndw.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ilm.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nep.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://kni.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://evs.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nim.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pra.smart0.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://jrd.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nvj.hnqzz.top

[I05] 按正则拆分
来源：http://bnv.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fzx.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://doe.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://itz.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://avo.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://fud.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zvb.cashguo.top

Ruby: s.split(/\s*,\s*/)
来源：http://hbj.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wfn.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bch.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aye.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://urk.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bfk.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldu.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kme.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lvs.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://acq.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://isl.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://ggc.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fvy.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pkf.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ikh.shanyushiyangkeji.top

TS:   /error/gim
来源：http://vtn.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hbe.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://exo.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://jwl.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jff.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://cpr.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nrt.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jym.aibaodan.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqy.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uws.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://kmf.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bkp.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ibw.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qlt.sxryk.cn

================================================================================
来源：http://vll.zhoulong.xyz

J. 日期与时间
来源：http://jhk.hcnkem.com

================================================================================
来源：http://ley.yj202588.top

[J01] 获取当前时间
来源：http://cni.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://icp.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aib.sweek.top

JS:   new Date();  Date.now()
来源：http://gjj.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://iku.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qdj.havefunace.top

Go:   time.Now()
来源：http://mdx.ctjpmb.com

Ruby: Time.now
来源：http://eoc.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qtn.hfpthk.cn

[J02] 格式化输出
来源：http://mgt.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ojw.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://chf.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nif.zdqjudy.top

TS:   d.toISOString()
来源：http://fnx.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ine.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dml.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zba.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pqu.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://ecr.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vua.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tou.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://tlw.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://mfw.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kxy.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wgs.jinyuanbaomall.cn

Ruby: Date.parse("2024-01-02")
来源：http://fem.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fdm.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://psu.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iad.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qoy.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bwr.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yrj.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jop.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ltp.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mip.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tgv.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://rub.tarul.cn

Py:   now + timedelta(days=7)
来源：http://ekd.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wqh.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mok.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ocp.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://qqk.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tan.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://roc.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bnq.316326.xyz

[J06] 计算两时间之差
来源：http://krq.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://cua.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://rkv.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wno.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bok.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://qrf.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://ihc.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://pmq.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://eib.mhx1999.top

[J07] 比较两个日期
来源：http://tac.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://udt.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yof.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wfw.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://cqo.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uvq.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dke.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://whm.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://hvh.ydzc1.top

[J08] 提取年月日与星期
来源：http://fua.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bnn.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mep.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ogn.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hjf.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bht.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ghu.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bks.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rvg.zdqjudy.top

[J09] 时区处理
来源：http://vjv.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nmc.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ezt.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdw.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://szr.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tus.cheryme.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hpv.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gso.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://acp.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://vsd.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://krs.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gjh.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cuz.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vbe.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qdb.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zzv.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ubw.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gfw.epnwcf.com

================================================================================
来源：http://msw.zhiwuduotai.top

K. JSON 与序列化
来源：http://xgq.daria6918.cn

================================================================================
来源：http://kdx.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://rns.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sre.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xev.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://unm.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://mpc.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mwy.xylfe.cn

Go:   json.Marshal(obj)
来源：http://iml.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://awp.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ekr.fehbvm.com

[K02] JSON 字符串转对象
来源：http://icl.haohaochexian.top

Py:   json.loads(s)
来源：http://zof.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zws.cashguo.top

JS:   JSON.parse(s)
来源：http://qdc.jiagoushi.top

TS:   JSON.parse(s)
来源：http://aqf.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kqu.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://vkg.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://rfz.gogol.net.cn


<!-- 参考信息 -->