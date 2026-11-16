代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://tjh.epnwcf.com

Java: record User(String name, int age) {}
来源：http://hqx.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://sna.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dlt.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://bqh.yj20258888.top

[G15] 枚举
来源：http://gkp.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://krb.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://apo.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uue.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kqz.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://msv.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://svq.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://pna.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://met.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://iao.cheryme.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jok.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://vqs.dianchejie.cn

JS:   Object.entries(obj)
来源：http://vue.haohaochexian.top

TS:   Object.entries(obj)
来源：http://rhm.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iux.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://jna.tianlin.xyz

Ruby: obj.instance_variables
来源：http://hwa.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://kvy.9152youxi.cn

================================================================================
来源：http://qhr.aizwys.cn

H. 异常与错误处理
来源：http://sbp.hywenlv.cn

================================================================================
来源：http://uqf.zycfv.cn

[H01] try / catch 基础
来源：http://crt.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sex.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://npr.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://unh.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gix.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zmm.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pib.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zdp.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fxi.sysykeji.top

[H02] finally / ensure 收尾
来源：http://ioe.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vva.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vwd.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hxz.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hys.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tnv.yongpay.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eas.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://erj.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nuq.ydzc1.top

[H03] 主动抛出异常
来源：http://esd.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://egx.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jen.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://ytl.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://kbw.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cdr.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hyl.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kyi.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://isj.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://des.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://fvd.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gvc.hammf.cn

JS:   class MyError extends Error {}
来源：http://svv.hesvh.cn

TS:   class MyError extends Error {}
来源：http://ybn.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://jcu.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wgk.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://skd.hesvh.cn

C#:   class MyException : Exception {}
来源：http://igt.nanxinkj.top

[H05] 捕获特定类型
来源：http://dpj.52xcode.cn

Py:   except ValueError as e:
来源：http://nle.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vwf.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://zsq.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://fok.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://xap.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mpw.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://fbi.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://quv.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://zre.sweek.top

Py:   value = d.get("k") or default
来源：http://xtw.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tjj.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://aec.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hlq.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mzc.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pfd.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://mbg.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://wzs.vqdsnc.cn

[H07] 断言
来源：http://yyo.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://afx.hfpthk.cn

PHP:  assert($x > 0);
来源：http://gmh.havefunace.top

JS:   console.assert(x > 0);
来源：http://qlw.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://lda.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://pdv.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tsg.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://tex.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://uyp.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://aji.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://lly.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ssq.mhx1999.top

JS:   e.message;  e.stack
来源：http://bor.epnwcf.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://fvn.redwolf501.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mli.hesvh.cn

Go:   err.Error()
来源：http://cux.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://twl.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://phs.redwolf501.top

[H09] 带错误码的异常
来源：http://ssv.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xnv.yj20258888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fdu.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zhe.0kj1m.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fhu.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zwb.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vbd.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://iko.shanyushiyangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xgr.daria6918.cn

[H10] 资源自动释放
来源：http://egf.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kda.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://awt.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vsn.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://upn.cqqwz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yqq.meibo888.top

Go:   defer f.Close()
来源：http://vhv.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qzv.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wme.redwolf501.top

================================================================================
来源：http://pbm.fehbvm.com

I. 正则表达式
来源：http://fxe.guowangkeji.top

================================================================================
来源：http://gaw.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://kzs.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hqb.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://fkm.wangdashe.top

JS:   /\d+/.test(s)
来源：http://ybh.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://jte.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://thy.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://efy.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://uee.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xld.tian-w.cn

[I02] 提取所有匹配
来源：http://ojx.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://nfa.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xiy.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rip.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://kdx.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cqg.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://osv.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://zqt.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://koj.kuanghao11.cn

[I03] 提取捕获分组
来源：http://wza.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ddi.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vtf.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zth.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mpr.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://olk.yfazqb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vvd.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ruh.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eye.jinyuanbaomall.cn

[I04] 正则替换
来源：http://jsw.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ilk.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://woo.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://lkr.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://jar.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://ims.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://yau.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ele.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://psh.yj20258.top

[I05] 按正则拆分
来源：http://prn.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jsw.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jfe.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://aqu.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://ekk.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://ewt.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vnm.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nct.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aca.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kuz.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lmw.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zvv.pengpengdd.cyou

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qph.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oqm.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yxy.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xmg.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ree.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jsc.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://irg.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xhd.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iog.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hzp.ybcxt.top

TS:   /error/gim
来源：http://hqi.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oih.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tkk.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://pdx.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wvd.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://cxm.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rpr.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ixi.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kxs.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ppc.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pvf.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://egg.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tgu.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wfm.andypj.xyz

================================================================================
来源：http://jph.kuanghao11.cn

J. 日期与时间
来源：http://jrr.yanxiufei.cn

================================================================================
来源：http://nrq.uphjek.com

[J01] 获取当前时间
来源：http://dum.shangyingyoupin.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pzv.sufxvd.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://npq.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://rwr.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://jnx.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rnc.hnqzz.top

Go:   time.Now()
来源：http://ess.zhoulong.xyz

Ruby: Time.now
来源：http://eog.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bdj.yongpay.top

[J02] 格式化输出
来源：http://kte.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hvi.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://myl.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xpq.tianlin.xyz

TS:   d.toISOString()
来源：http://hlr.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yje.ydzc1.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ulc.zhaomingkeji.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ntm.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://neq.gzhubu.top

[J03] 字符串解析为日期
来源：http://osq.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://exo.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lur.yj20258.top

JS:   new Date("2024-01-02")
来源：http://qwy.havefunace.top

TS:   new Date("2024-01-02")
来源：http://nwc.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://spc.hesvh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://omx.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://laa.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qel.smart0.xyz

[J04] 时间戳与日期互转
来源：http://vbt.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://far.316326.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ehu.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://axb.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://vue.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bpt.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ywo.cqqwz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://egn.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bqj.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://llk.birdmap.top

Py:   now + timedelta(days=7)
来源：http://sow.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tux.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wfx.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yry.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://aky.shzxlz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oaq.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://iss.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://yee.hcnkem.com

[J06] 计算两时间之差
来源：http://pyb.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://ejg.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://koq.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://phb.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uuk.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://haz.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://rzn.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://jdm.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://rxp.c1oappe.top

[J07] 比较两个日期
来源：http://utc.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://gqa.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ayx.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://xvn.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rws.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uzr.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wtl.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://cio.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://eji.fktsv.cn

[J08] 提取年月日与星期
来源：http://csl.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://liz.xuetiantiany.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://csx.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jzs.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nbh.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sqc.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lru.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rra.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ktm.jqgufenzy.top

[J09] 时区处理
来源：http://oqx.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pxj.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qjx.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jra.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fda.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://juu.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ewd.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xve.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eqr.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://dbe.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jav.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sqw.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gan.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rsf.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bef.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://flb.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rdg.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qhb.gaohongyu789.top

================================================================================
来源：http://jcb.hcnkem.com

K. JSON 与序列化
来源：http://dbk.zdqjudy.top

================================================================================
来源：http://rqk.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://oar.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xek.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xaa.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://tfh.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://yka.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aon.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://cjy.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://yme.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lhp.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://zmv.shuidangran.top

Py:   json.loads(s)
来源：http://gys.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tjk.sufxvd.cn

JS:   JSON.parse(s)
来源：http://znu.sxryk.cn


<!-- 参考信息 -->