代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://ihx.andypj.xyz

Java: record User(String name, int age) {}
来源：http://msv.cdnleiting.top

Go:   type User struct { Name string; Age int }
来源：http://rbl.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zwr.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://woe.hongshengwenyu.top

[G15] 枚举
来源：http://ywu.hnxiangtu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pck.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hpy.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://frd.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iqm.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://stn.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zyj.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://oll.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jbx.ivvv.top

[G16] 对象转数组 / 字典
来源：http://vsn.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bmt.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://hgt.ivvv.top

JS:   Object.entries(obj)
来源：http://znv.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://ahc.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ggj.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ukn.yfazqb.com

Ruby: obj.instance_variables
来源：http://usl.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://unl.svipenyu.cn

================================================================================
来源：http://wyp.xziqi.cn

H. 异常与错误处理
来源：http://mlh.hongshengwenyu.top

================================================================================
来源：http://ign.zhijiandao.cn

[H01] try / catch 基础
来源：http://bfn.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pmj.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wai.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hew.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bjd.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xfo.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gmw.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zmy.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://alj.meibo888.top

[H02] finally / ensure 收尾
来源：http://dpr.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://emt.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ult.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rlb.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://iwc.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wcc.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gva.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ern.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://agq.havefunace.top

[H03] 主动抛出异常
来源：http://byp.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://pyk.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qmp.cashguo.top

JS:   throw new Error("错误信息");
来源：http://zbw.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://ewu.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vrb.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tmu.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xxi.shzxlz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mkt.hnqzz.top

[H04] 自定义异常类型
来源：http://fqp.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://ejy.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://hig.yvedp.cn

JS:   class MyError extends Error {}
来源：http://bxr.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://npd.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://kef.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ufl.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://hca.guannengcc.top

C#:   class MyException : Exception {}
来源：http://hzh.ivvv.top

[H05] 捕获特定类型
来源：http://ata.cheryme.top

Py:   except ValueError as e:
来源：http://emj.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dfh.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://mtu.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://oym.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://kgx.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sxj.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://pti.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mbw.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://miq.bjfxy.top

Py:   value = d.get("k") or default
来源：http://eps.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://eue.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://cvw.yangfankeji.com

TS:   obj?.a?.b;  d ?? default
来源：http://rts.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://frq.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yvv.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://wrj.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://dyk.yangfankeji.com

[H07] 断言
来源：http://pkf.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://uni.jqgfzy.top

PHP:  assert($x > 0);
来源：http://dzm.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://cvu.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://vwy.jinyuanbaomall.cn

Java: assert x > 0 : "必须为正";
来源：http://dja.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gqr.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://pau.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://tqi.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://jqr.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://wpp.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lzh.yuanzhike.top

JS:   e.message;  e.stack
来源：http://dsl.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://rqg.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://thy.9152youxi.cn

Go:   err.Error()
来源：http://auj.xziqi.cn

Ruby: e.message;  e.backtrace
来源：http://tgw.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://uxc.andypj.xyz

[H09] 带错误码的异常
来源：http://exq.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lhr.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vma.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jqd.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pkn.jinqigfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dvt.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ivd.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vvu.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vwv.daxiang520.top

[H10] 资源自动释放
来源：http://oqv.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fpj.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vcw.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sss.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://byp.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://smr.pycfn.com

Go:   defer f.Close()
来源：http://via.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hja.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hdf.xuetiantiany.cn

================================================================================
来源：http://nvk.ehwqpu.com

I. 正则表达式
来源：http://ikh.fktsv.cn

================================================================================
来源：http://uyr.jiagoushi.top

[I01] 判断是否匹配
来源：http://gqv.jinyuanbaomall.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jsl.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lxu.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://ent.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://jnj.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://npw.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ruj.ybcxt.top

Ruby: s.match?(/\d+/)
来源：http://bkb.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nlh.jianghu66.top

[I02] 提取所有匹配
来源：http://ain.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://svu.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kbz.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jrp.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://ewd.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nva.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qqg.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://azg.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://inm.chenzaomai.com

[I03] 提取捕获分组
来源：http://dhh.316326.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uig.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aul.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://npy.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kox.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kmt.bbcook.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pxk.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yac.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tfx.feifeiyinyue.top

[I04] 正则替换
来源：http://dyq.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gvf.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ohz.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vli.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://mol.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://hla.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ont.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://rcd.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yzg.feifeiyinyue.top

[I05] 按正则拆分
来源：http://kws.daria6918.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rqi.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pyj.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://kmg.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ntx.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://rod.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://glg.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://iyw.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cfc.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://usk.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fyb.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xzl.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://exx.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oig.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bgk.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dki.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qeo.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hks.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://jkj.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://axt.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ghk.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zol.snrcjt.cn

TS:   /error/gim
来源：http://tan.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cgh.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jvc.gotoacloud.top

Ruby: s.scan(/error/i)
来源：http://pnr.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qeh.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://chf.chenlongwang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qjm.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zcr.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gdk.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ldf.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fec.ehwqpu.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gmz.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ipk.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sgc.sweek.top

================================================================================
来源：http://pkk.jinghuilouyu.cn

J. 日期与时间
来源：http://tob.pengpengdd.cyou

================================================================================
来源：http://wkq.guowangkeji.top

[J01] 获取当前时间
来源：http://qlw.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mxa.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pxp.zycfv.cn

JS:   new Date();  Date.now()
来源：http://cnn.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://waq.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ndy.jyoumei.cn

Go:   time.Now()
来源：http://mlk.zycfv.cn

Ruby: Time.now
来源：http://rnz.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jps.ybcxt.top

[J02] 格式化输出
来源：http://pmu.svipenyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ipn.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://caq.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uyf.ivvv.top

TS:   d.toISOString()
来源：http://lbx.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cvo.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jrj.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pcx.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://czk.52xcode.cn

[J03] 字符串解析为日期
来源：http://ywk.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://awn.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bct.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://stm.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://czw.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ygy.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yrl.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://kse.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rzc.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://qxr.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ypr.sufxvd.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uer.sufxvd.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yjw.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://noe.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pmm.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cqr.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://doa.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zmc.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://rgi.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://aqy.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uzr.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ard.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvs.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://exv.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jwb.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://gqh.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zil.shzxlz.cn

[J06] 计算两时间之差
来源：http://zwv.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://unn.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://qse.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://els.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://whq.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ooa.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://sdz.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://kkj.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://zoh.cashguo.top

[J07] 比较两个日期
来源：http://orc.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://lnn.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://avn.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://vph.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://xpi.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lqc.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kgo.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://vld.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://xfs.ppjwa.cn

[J08] 提取年月日与星期
来源：http://oka.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgc.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fvf.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gjc.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://idh.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tgq.cucudq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yjm.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qhx.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nfo.yj20258888.top

[J09] 时区处理
来源：http://chh.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tml.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nfa.0kj1m.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ifk.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hwh.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gne.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fpw.jyoumei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vtc.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rnu.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://kpj.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://byy.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xor.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://quo.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nww.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zno.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rwj.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pds.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tta.tianlin.xyz

================================================================================
来源：http://mkd.meibo888.top

K. JSON 与序列化
来源：http://euy.jianghu66.top

================================================================================
来源：http://yid.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://nyi.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hki.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jcd.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://eve.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://ihe.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://evt.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://xvr.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://onq.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://cmq.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://tzh.iojbl.cn

Py:   json.loads(s)
来源：http://rze.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lqu.yuxming.cn

JS:   JSON.parse(s)
来源：http://gph.vqdsnc.cn


<!-- 参考信息 -->