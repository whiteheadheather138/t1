代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://pxb.hesvh.cn

Java: record User(String name, int age) {}
来源：http://iof.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://cxq.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bti.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://mkr.xinyue.icu

[G15] 枚举
来源：http://teu.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jqh.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://qxa.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qtu.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xqr.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://yex.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vcu.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://pdn.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ugi.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://bdc.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xfz.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://rur.tarul.cn

JS:   Object.entries(obj)
来源：http://ioz.iojbl.cn

TS:   Object.entries(obj)
来源：http://yxv.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vls.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://otq.ybcxt.top

Ruby: obj.instance_variables
来源：http://jng.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://pwm.yvedp.cn

================================================================================
来源：http://wui.hcnkem.com

H. 异常与错误处理
来源：http://auu.cashguo.top

================================================================================
来源：http://umr.shuidangran.top

[H01] try / catch 基础
来源：http://rtn.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ixm.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vix.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://coq.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gto.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tav.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hqv.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kxp.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://viw.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://sbq.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://frf.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yqz.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pmn.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cck.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zxp.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://orx.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://urk.aibaodan.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qso.yonumen.top

[H03] 主动抛出异常
来源：http://qtb.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://bix.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kny.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://zbf.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://vbf.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://drp.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mjt.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yqo.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ktc.bbcook.cn

[H04] 自定义异常类型
来源：http://uni.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://nsx.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hzy.ywan-chungtsiang.top

JS:   class MyError extends Error {}
来源：http://cgw.fehbvm.com

TS:   class MyError extends Error {}
来源：http://dyy.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://izz.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qms.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://mnx.cheryme.top

C#:   class MyException : Exception {}
来源：http://bru.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://yvi.nanxinkj.top

Py:   except ValueError as e:
来源：http://dqy.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jfg.zhoulong.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ghv.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://ymx.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://ozy.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qbf.sxryk.cn

Ruby: rescue ArgumentError => e
来源：http://ygn.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tsh.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://qlg.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://rco.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ebw.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://scb.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://rti.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fuc.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jho.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://rzn.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://qvc.ywan-chungtsiang.top

[H07] 断言
来源：http://rxn.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://nso.haohaochexian.top

PHP:  assert($x > 0);
来源：http://muo.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://poj.fehbvm.com

TS:   console.assert(x > 0);
来源：http://kmf.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://lzs.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gpa.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kpk.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://wbv.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://nbd.yfazqb.com

Py:   str(e);  traceback.format_exc()
来源：http://ssb.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nvi.zdbjq.cn

JS:   e.message;  e.stack
来源：http://ncn.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vgm.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://pss.jqgufenzy.top

Go:   err.Error()
来源：http://uiw.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://lqp.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://dzg.nwbrower.top

[H09] 带错误码的异常
来源：http://cdk.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://agw.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ehu.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kgy.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eon.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cyp.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hlm.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://tdw.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://erk.zdbjq.cn

[H10] 资源自动释放
来源：http://vcd.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lnr.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fkx.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vmt.xuanzx.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iwa.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://buh.chenjidiqi.icu

Go:   defer f.Close()
来源：http://vcr.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fip.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tcq.zhaomingkeji.xyz

================================================================================
来源：http://jff.svipenyu.cn

I. 正则表达式
来源：http://bry.yfazqb.com

================================================================================
来源：http://yji.316326.xyz

[I01] 判断是否匹配
来源：http://uyi.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vwj.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://yub.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://ztz.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://hyi.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ohr.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rcm.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://pjb.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ujf.ydjk.org.cn

[I02] 提取所有匹配
来源：http://nsq.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://jxp.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fpv.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nja.zhengqikj.top

TS:   s.match(/\d+/g)
来源：http://rzo.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nyb.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yxo.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://xco.zhoulong.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qkx.cqqwz.cn

[I03] 提取捕获分组
来源：http://xkz.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qzr.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://asm.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gpj.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://stu.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://unu.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wuw.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bwq.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iro.yongpay.top

[I04] 正则替换
来源：http://pwk.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://vxy.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kxm.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://czy.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tdi.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://shc.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://llr.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://wis.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sfz.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://apc.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oha.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hwn.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://ntj.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://gtg.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://nam.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wjk.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://cro.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://evl.havefunace.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hmp.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dlp.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jbd.cdnleiting.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kri.9152youxi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rer.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qzi.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sap.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhu.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gsy.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://hky.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nda.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mst.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cfc.hongshengwenyu.top

TS:   /error/gim
来源：http://rpa.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vef.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://htt.meibo888.top

Ruby: s.scan(/error/i)
来源：http://gbq.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wnj.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://hxx.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vlm.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://clr.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mxd.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jgs.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://zva.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qer.zdqjudy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ntz.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aai.yuanzhike.top

================================================================================
来源：http://moz.zhongyouzk.top

J. 日期与时间
来源：http://ivw.zdqjudy.top

================================================================================
来源：http://rtj.aibaodan.cn

[J01] 获取当前时间
来源：http://nty.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fye.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cpu.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://evj.cashguo.top

TS:   new Date();  Date.now()
来源：http://zxi.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tsk.shzxlz.cn

Go:   time.Now()
来源：http://rxs.kuanghao11.cn

Ruby: Time.now
来源：http://lcw.hnxiangtu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bst.daria6918.cn

[J02] 格式化输出
来源：http://dwu.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://evq.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nfh.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nkp.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://kvv.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hpe.ehwqpu.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xpy.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ifx.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://art.hcnkem.com

[J03] 字符串解析为日期
来源：http://yhx.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nrn.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pbc.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://mzp.ivvv.top

TS:   new Date("2024-01-02")
来源：http://hqc.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://fli.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fik.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://rof.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bgt.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://sma.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iet.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://duu.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qse.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://luf.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jev.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xxp.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rpb.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sno.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://vek.tarul.cn

Py:   now + timedelta(days=7)
来源：http://stk.fanxiaobao.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ggf.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uuc.jianghu66.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kab.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://lyx.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://aui.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://won.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://qwn.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://cwh.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://ybn.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://htz.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eoq.epnwcf.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://drb.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://opf.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://fca.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://etk.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://ewj.nwbrower.top

[J07] 比较两个日期
来源：http://nqg.zhoulong.xyz

Py:   d1 < d2;  d1 == d2
来源：http://xqd.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bmz.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://ehk.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://gzo.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pqh.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wjp.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kwf.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://yel.xziqi.cn

[J08] 提取年月日与星期
来源：http://ckk.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fdu.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dkf.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ojx.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kdd.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zyk.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://frb.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ogx.sufxvd.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qdl.feifeiyinyue.top

[J09] 时区处理
来源：http://utf.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zfr.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dyd.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mmb.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vig.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mtc.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xyd.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jno.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zld.0kj1m.cn

[J10] 取今天 / 本月第一天
来源：http://awz.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ork.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dlf.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nxz.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xsn.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zkk.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ppx.snrcjt.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ngs.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://afr.dashuyun.cn

================================================================================
来源：http://hmc.jianghu66.top

K. JSON 与序列化
来源：http://iva.hfpthk.cn

================================================================================
来源：http://wea.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://fbh.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vfc.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rnw.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://mrx.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://vby.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ysq.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://nzv.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wtb.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jxd.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://fuy.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://ixm.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ocy.ehwqpu.com

JS:   JSON.parse(s)
来源：http://rxa.snrcjt.cn


<!-- 参考信息 -->