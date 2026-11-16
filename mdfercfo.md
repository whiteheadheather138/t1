代发 wailian999

[G14] 数据类 / record
来源：http://vrm.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eto.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://vuw.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://esn.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://vsb.smart0.xyz

Java: record User(String name, int age) {}
来源：http://nwe.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://ldt.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bnv.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://igq.gzhubu.top

[G15] 枚举
来源：http://yrx.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jzp.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ziz.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qqn.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ybg.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://vjs.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fgx.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://ryi.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uhk.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://wic.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zlv.jiagoushi.top

PHP:  get_object_vars($obj);
来源：http://whf.zycfv.cn

JS:   Object.entries(obj)
来源：http://jdq.gogol.net.cn

TS:   Object.entries(obj)
来源：http://hdj.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jvx.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lvw.chenzaomai.com

Ruby: obj.instance_variables
来源：http://syz.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://efp.zhengqikj.top

================================================================================
来源：http://yjm.hammf.cn

H. 异常与错误处理
来源：http://srh.nanxinkj.top

================================================================================
来源：http://qte.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://djs.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://szx.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ezu.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dji.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pjp.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sgp.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rqw.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://clr.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hdy.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://gqa.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://lfr.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wth.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wjy.zhongyouzk.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lkv.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gzv.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://bev.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ugz.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bqv.tianlin.xyz

[H03] 主动抛出异常
来源：http://czz.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://kqz.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fey.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://ngt.zhoulong.xyz

TS:   throw new Error("错误信息");
来源：http://opf.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://frz.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fop.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dfx.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://bpa.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://ekp.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://zgi.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://zoe.fktsv.cn

JS:   class MyError extends Error {}
来源：http://qoa.yueranfly.top

TS:   class MyError extends Error {}
来源：http://xtt.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://fqg.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fzf.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://rdi.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://qql.zhixingplan.top

[H05] 捕获特定类型
来源：http://hhs.zhaomingkeji.xyz

Py:   except ValueError as e:
来源：http://kgz.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cca.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://oig.yongpay.top

TS:   if (e instanceof TypeError) {}
来源：http://xeu.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://blp.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gqm.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://zzr.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dlk.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://yzw.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://pjh.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://dap.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://kco.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://nea.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pxv.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fxd.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://tbw.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://svj.dianchejie.cn

[H07] 断言
来源：http://upc.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://vkc.uphjek.com

PHP:  assert($x > 0);
来源：http://jgu.iojbl.cn

JS:   console.assert(x > 0);
来源：http://mku.yfazqb.com

TS:   console.assert(x > 0);
来源：http://tte.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://kwt.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jvd.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://zhn.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://gti.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://rlv.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://hwg.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uzb.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://jag.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://nxe.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tfu.hnxiangtu.top

Go:   err.Error()
来源：http://nje.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://ytp.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://rsj.daxiang520.top

[H09] 带错误码的异常
来源：http://wvj.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qkb.zycfv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://coz.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mnl.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://epm.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tmt.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zqp.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gbp.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rbw.jyoumei.cn

[H10] 资源自动释放
来源：http://dsz.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://svu.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dim.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://guh.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nat.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wht.quarkkingdee.top

Go:   defer f.Close()
来源：http://hma.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fqa.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iyk.jinqigufen.top

================================================================================
来源：http://suy.daxiang520.top

I. 正则表达式
来源：http://cmh.andypj.xyz

================================================================================
来源：http://sgc.gaohongyu789.top

[I01] 判断是否匹配
来源：http://ahk.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ecz.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gnx.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://gup.hesvh.cn

TS:   /\d+/.test(s)
来源：http://glw.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rok.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://svv.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://okx.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rof.yanxiufei.cn

[I02] 提取所有匹配
来源：http://crc.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://mtf.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vpc.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qxk.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://ssd.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ekn.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sdq.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://pbf.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://frb.dashuyun.cn

[I03] 提取捕获分组
来源：http://iwv.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lrp.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wuj.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iib.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yvh.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qui.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yds.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zjb.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kaa.shanyushiyangtech.top

[I04] 正则替换
来源：http://efv.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ifq.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gln.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ksi.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://zee.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://kqr.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gde.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cre.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://czd.yj20258.top

[I05] 按正则拆分
来源：http://ytk.jinghuilouyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lue.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://krc.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://fkn.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ayh.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://fjw.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://thk.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nwq.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dyh.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hjl.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pad.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://beh.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dvj.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rlh.bbcook.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wls.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ioa.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wxo.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yit.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://mhw.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eyw.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iay.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xqg.316326.xyz

TS:   /error/gim
来源：http://odj.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rne.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uii.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://ahv.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cgn.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://hwt.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lua.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rqi.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nuf.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://omo.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://psy.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aml.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ekm.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ujl.fzhhl.top

================================================================================
来源：http://ayk.zycfv.cn

J. 日期与时间
来源：http://lij.sjlbkw.cn

================================================================================
来源：http://drz.yanxiufei.cn

[J01] 获取当前时间
来源：http://zfr.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bol.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tzh.cucudq.cn

JS:   new Date();  Date.now()
来源：http://eec.fehbvm.com

TS:   new Date();  Date.now()
来源：http://zfg.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zcr.fanxiaobao.xyz

Go:   time.Now()
来源：http://uaj.yueranfly.top

Ruby: Time.now
来源：http://emt.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nsi.316326.xyz

[J02] 格式化输出
来源：http://tuh.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xti.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xbi.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ovu.9152youxi.cn

TS:   d.toISOString()
来源：http://vhd.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://thy.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://udz.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hcg.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xni.ctjpmb.com

[J03] 字符串解析为日期
来源：http://wuk.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://scz.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fdw.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://tdn.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://hgj.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xrx.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kjd.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://jpf.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qaw.bbcook.cn

[J04] 时间戳与日期互转
来源：http://kjq.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pjr.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fus.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cye.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kkg.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://veb.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pxb.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kpd.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bfa.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://uiy.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://yzf.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uyr.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tcu.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://joy.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://dms.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rra.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://hzr.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pjv.yangfankeji.com

[J06] 计算两时间之差
来源：http://uja.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://zvt.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://zfx.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qsd.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mrb.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://epn.vqdsnc.cn

Go:   end.Sub(start).Hours()
来源：http://iku.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://jtm.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://pzr.epnwcf.com

[J07] 比较两个日期
来源：http://oem.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://mml.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tty.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://fje.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://wxl.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bkc.ctjpmb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sfi.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://ifv.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://bhy.ivvv.top

[J08] 提取年月日与星期
来源：http://qia.jinqigufen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xla.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kpq.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://elg.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ayd.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qeh.aizwys.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nty.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ezo.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rur.hfpthk.cn

[J09] 时区处理
来源：http://rdp.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://umn.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rpd.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vxf.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jwd.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jkm.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://viv.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ruh.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://awl.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://osp.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zza.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lqb.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dcd.ctjpmb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uey.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ywi.wangshuangyany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://del.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mwg.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iyj.gaohongyu789.top

================================================================================
来源：http://cmk.fanxiaobao.xyz

K. JSON 与序列化
来源：http://hky.52xcode.cn

================================================================================
来源：http://cre.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://dvw.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jdf.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xaa.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://krr.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://wkn.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yrh.yj202588.top

Go:   json.Marshal(obj)
来源：http://pjt.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://vjk.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rgt.zycfv.cn


<!-- 参考信息 -->