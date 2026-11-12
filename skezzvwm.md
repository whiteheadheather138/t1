代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kbs.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hhj.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://cnd.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zlt.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://hyn.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lem.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://bkk.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sum.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://tlu.nwbrower.top

JS:   Object.entries(obj)
来源：http://mmh.zhengqikj.top

TS:   Object.entries(obj)
来源：http://nrx.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ynd.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://awq.yj20258888.top

Ruby: obj.instance_variables
来源：http://jmf.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://xlw.jinqigufen.top

================================================================================
来源：http://kln.meibo888.top

H. 异常与错误处理
来源：http://vei.hcnkem.com

================================================================================
来源：http://ykl.dianchejie.cn

[H01] try / catch 基础
来源：http://uot.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uju.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tsq.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cvh.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nzr.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://otr.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kkp.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fjd.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eia.fzhhl.top

[H02] finally / ensure 收尾
来源：http://poo.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://xyi.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://myc.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jem.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rct.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://fzy.hesvh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oob.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fpv.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vba.0kj1m.cn

[H03] 主动抛出异常
来源：http://ygi.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://ttt.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://equ.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://lhd.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://qpw.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://dmq.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ajg.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qvy.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://yic.vehdjk.com

[H04] 自定义异常类型
来源：http://dwh.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://cso.ywan-chungtsiang.top

PHP:  class MyError extends RuntimeException {}
来源：http://whh.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://vtu.uphjek.com

TS:   class MyError extends Error {}
来源：http://wqp.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://uik.chenlongwang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kvy.fktsv.cn

Ruby: class MyError < StandardError; end
来源：http://iyl.daxiang520.top

C#:   class MyException : Exception {}
来源：http://wlk.tarul.cn

[H05] 捕获特定类型
来源：http://ehy.meibo888.top

Py:   except ValueError as e:
来源：http://hkn.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xiv.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://etq.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://wdi.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://axv.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rfe.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://rsp.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qwb.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://dqe.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://txw.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rnn.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nzg.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://amz.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://thv.nwbrower.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xkz.meibo888.top

Ruby: d&.dig(:a, :b)
来源：http://eke.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://rsj.sweek.top

[H07] 断言
来源：http://got.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://iwm.gotoacloud.top

PHP:  assert($x > 0);
来源：http://cum.sweek.top

JS:   console.assert(x > 0);
来源：http://imr.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://ngt.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://qwq.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gzu.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://yeb.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://gcp.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://ggw.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://wbe.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ydo.wangdashe.top

JS:   e.message;  e.stack
来源：http://llq.yfazqb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://btl.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pvx.hammf.cn

Go:   err.Error()
来源：http://ecm.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://iuw.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://gqk.fehbvm.com

[H09] 带错误码的异常
来源：http://hhw.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mfj.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wyh.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bhx.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jtt.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gjx.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sha.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://ues.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ouo.birdmap.top

[H10] 资源自动释放
来源：http://tem.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wbi.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oou.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://woh.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zkv.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iqo.ivvv.top

Go:   defer f.Close()
来源：http://hil.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lzx.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://swc.bbcook.cn

================================================================================
来源：http://wso.xinyue.icu

I. 正则表达式
来源：http://klw.ppjwa.cn

================================================================================
来源：http://awk.quarkkingdee.top

[I01] 判断是否匹配
来源：http://rwo.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jni.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://jei.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://jxl.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://vxs.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wmx.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sid.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://iiz.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ecl.jqgufenzy.top

[I02] 提取所有匹配
来源：http://txb.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://noo.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ddv.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nbn.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://rhp.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xts.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ild.fktsv.cn

Ruby: s.scan(/\d+/)
来源：http://wsz.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qpi.andypj.xyz

[I03] 提取捕获分组
来源：http://tvv.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qlr.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iop.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ugi.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mde.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hyg.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ztm.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zyn.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nhw.epnwcf.com

[I04] 正则替换
来源：http://xff.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cdz.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sfl.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nlj.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mls.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://buq.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vyd.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mxi.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pve.mhx1999.top

[I05] 按正则拆分
来源：http://yks.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dnh.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iud.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://qyz.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://scs.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://sfj.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xen.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ebz.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zoa.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gpw.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jlu.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rqy.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://veo.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qsy.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zld.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wij.hesvh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bhz.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ijj.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://nxw.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yad.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vwd.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vlu.tianlin.xyz

TS:   /error/gim
来源：http://nwy.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://azs.vqdsnc.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fso.xuanzx.com

Ruby: s.scan(/error/i)
来源：http://pnn.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qym.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://suk.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kez.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wof.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pxi.ehwqpu.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aru.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rvu.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zyi.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ssu.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://byh.guowangkeji.top

================================================================================
来源：http://tke.hnqzz.top

J. 日期与时间
来源：http://wrm.tanke756.top

================================================================================
来源：http://dkt.ydjk.org.cn

[J01] 获取当前时间
来源：http://cga.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://esf.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ggh.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://wkk.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://cul.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zyy.ydjk.org.cn

Go:   time.Now()
来源：http://izb.hnqzz.top

Ruby: Time.now
来源：http://exu.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lka.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://usv.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://azt.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wex.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wzk.tianlin.xyz

TS:   d.toISOString()
来源：http://tfv.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tbh.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yvu.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lej.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eks.xuanzx.com

[J03] 字符串解析为日期
来源：http://kas.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vwp.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dfj.tanke756.top

JS:   new Date("2024-01-02")
来源：http://spk.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://pdw.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://zmy.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://owx.wangdashe.top

Ruby: Date.parse("2024-01-02")
来源：http://qzt.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xks.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://pwm.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rvq.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://crf.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://icj.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mcn.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nny.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tmj.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ngm.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hae.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://ooa.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://mpl.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://soo.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://omm.havefunace.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bkh.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://jbs.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xtc.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://ajg.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://lwv.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://ihv.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://sgt.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://eks.316326.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gge.ybcxt.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ita.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://rbn.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://wsx.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://trm.daria6918.cn

C#:   (end - start).TotalSeconds
来源：http://apk.hnqzz.top

[J07] 比较两个日期
来源：http://tvj.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://tun.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bqt.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vgj.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://esp.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ica.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mhq.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://znw.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://uqt.ehwqpu.com

[J08] 提取年月日与星期
来源：http://ktu.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://exj.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sgo.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lcp.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jfa.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lca.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fan.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eif.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zlg.bbcook.cn

[J09] 时区处理
来源：http://ytw.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yif.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hot.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zky.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://muu.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vse.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://edy.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fin.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wfc.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://rax.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ngr.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hbr.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mvx.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://agx.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hsc.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jhd.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jfq.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sfe.hywenlv.cn

================================================================================
来源：http://sxu.zdbjq.cn

K. JSON 与序列化
来源：http://acn.yuanzhike.top

================================================================================
来源：http://rqp.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://lkf.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wsi.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fpg.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://tkk.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://wsc.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sgx.yj202588.top

Go:   json.Marshal(obj)
来源：http://sjy.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://hxq.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://psr.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://xlg.jiagoushi.top

Py:   json.loads(s)
来源：http://xot.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mev.cqqwz.cn

JS:   JSON.parse(s)
来源：http://thw.birdmap.top

TS:   JSON.parse(s)
来源：http://lnk.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kak.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://hge.redwolf501.top

Ruby: JSON.parse(s)
来源：http://jri.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lse.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://vwd.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jol.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xhb.jiagoushi.top


<!-- 参考信息 -->