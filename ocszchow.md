代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xhy.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fqa.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://uyn.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fkt.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://kog.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gfo.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://num.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hph.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://gjn.zdbjq.cn

JS:   Object.entries(obj)
来源：http://ccb.hysaishi.cn

TS:   Object.entries(obj)
来源：http://nxr.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://een.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://gxb.fehbvm.com

Ruby: obj.instance_variables
来源：http://hjg.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://fyq.cqqwz.cn

================================================================================
来源：http://uwl.xuanzx.com

H. 异常与错误处理
来源：http://soi.yj202588.top

================================================================================
来源：http://lrg.xuanzx.com

[H01] try / catch 基础
来源：http://jmq.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://btg.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xwc.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://erc.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hzl.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rbj.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kip.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lhz.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wsd.hammf.cn

[H02] finally / ensure 收尾
来源：http://qjt.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://csc.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pov.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bjy.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fgu.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://vlt.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dvs.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sqa.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rxf.redwolf501.top

[H03] 主动抛出异常
来源：http://kui.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://ygk.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fbk.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://pth.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://fdx.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://glf.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dzf.fehbvm.com

Ruby: raise ArgumentError, "错误信息"
来源：http://xbc.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://vsc.yongpay.top

[H04] 自定义异常类型
来源：http://djr.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://pzm.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://akl.hesvh.cn

JS:   class MyError extends Error {}
来源：http://qzw.yongpay.top

TS:   class MyError extends Error {}
来源：http://lni.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://wkf.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nln.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://npr.shuidangran.top

C#:   class MyException : Exception {}
来源：http://zlz.ydjk.org.cn

[H05] 捕获特定类型
来源：http://zjs.0kj1m.cn

Py:   except ValueError as e:
来源：http://ltj.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tuy.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://wpp.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://zsq.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://auf.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yat.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://meh.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gwy.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://eip.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://ogp.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bdd.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zfo.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://vtd.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dvu.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wzi.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://wkw.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://leo.nanxinkj.top

[H07] 断言
来源：http://whz.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://seb.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://nqw.chenjidiqi.icu

JS:   console.assert(x > 0);
来源：http://vpz.yongpay.top

TS:   console.assert(x > 0);
来源：http://jxv.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://azb.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ajb.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jtb.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://xkp.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://exo.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://rqx.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lvs.zdqjudy.top

JS:   e.message;  e.stack
来源：http://oux.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dbs.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uqn.ehwqpu.com

Go:   err.Error()
来源：http://yjf.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://uvq.uphjek.com

C#:   e.Message;  e.StackTrace
来源：http://vwa.sysykeji.top

[H09] 带错误码的异常
来源：http://xrq.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yov.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gop.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xjf.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zlz.andypj.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uhl.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hfc.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dsl.52xcode.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://htq.haohaochexian.top

[H10] 资源自动释放
来源：http://ffn.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cge.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hwl.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wux.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ibh.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zgs.hnxiangtu.top

Go:   defer f.Close()
来源：http://bgd.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hkb.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bjr.chenlongwang.top

================================================================================
来源：http://ozs.xuanzx.com

I. 正则表达式
来源：http://zig.chenzaomai.com

================================================================================
来源：http://awm.nanxuanxn.top

[I01] 判断是否匹配
来源：http://qde.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xam.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rkh.ybcxt.top

JS:   /\d+/.test(s)
来源：http://vbg.cashguo.top

TS:   /\d+/.test(s)
来源：http://dgz.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hhy.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://awy.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://qcm.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kql.jianghu66.top

[I02] 提取所有匹配
来源：http://cwe.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://muk.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://umq.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cjh.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://zox.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dfw.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eyq.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://lyz.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zvp.cashguo.top

[I03] 提取捕获分组
来源：http://kst.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://osg.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cqh.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gji.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qcn.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oab.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://esu.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lje.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ohw.jiagoushi.top

[I04] 正则替换
来源：http://ntz.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tjw.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ahr.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://gxu.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://rcz.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://hgl.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qmi.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wsl.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://amp.yj202588.top

[I05] 按正则拆分
来源：http://imf.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://qli.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nlw.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://nuu.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://tts.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://ymq.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gqw.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://slm.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fgp.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ogs.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ivz.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lvb.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vbb.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://skn.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gzg.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lax.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vyd.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zme.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://kav.epnwcf.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wym.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://huh.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sec.yj202588.top

TS:   /error/gim
来源：http://bcm.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nyt.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xzx.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://jno.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xid.shzxlz.cn

[I08] 贪婪与非贪婪匹配
来源：http://jgd.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dik.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bzh.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bel.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eiv.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xrc.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nhq.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yly.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://huy.zhengqikj.top

================================================================================
来源：http://zxy.nwbrower.top

J. 日期与时间
来源：http://fah.hnqzz.top

================================================================================
来源：http://ahf.52xcode.cn

[J01] 获取当前时间
来源：http://sju.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pqb.xuanzx.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sbw.cucudq.cn

JS:   new Date();  Date.now()
来源：http://wxk.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://rmo.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ops.sweek.top

Go:   time.Now()
来源：http://moq.zdbjq.cn

Ruby: Time.now
来源：http://ybs.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://swa.hnqzz.top

[J02] 格式化输出
来源：http://kki.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xqg.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://taa.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ivm.fengsongda.top

TS:   d.toISOString()
来源：http://oiq.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pov.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dwb.52xcode.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pwk.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mrv.yj202588.top

[J03] 字符串解析为日期
来源：http://owk.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xrn.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kie.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://mcl.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://fpj.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hhx.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dif.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://gpp.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nmg.mhx1999.top

[J04] 时间戳与日期互转
来源：http://jdb.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rst.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bva.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sul.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://skd.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nfq.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://map.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mbo.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wtj.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://iro.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://acj.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://fro.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vuf.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xqz.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://jsp.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tod.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://ywi.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://mop.hesvh.cn

[J06] 计算两时间之差
来源：http://jst.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://mdi.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://hgn.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lpe.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zur.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://zdr.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://acw.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://aqi.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://ckh.yvedp.cn

[J07] 比较两个日期
来源：http://kaf.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://dgi.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kse.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://khu.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://pvn.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://emx.yuanzhike.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tlk.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://pex.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://fkg.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://dds.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rgv.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tpk.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ery.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://omx.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xyr.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pnl.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mbm.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://neg.cucudq.cn

[J09] 时区处理
来源：http://tkk.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aoo.yj202588.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kls.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vyd.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbv.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lmo.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bff.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ieg.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qwd.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://xch.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://onk.cdnleiting.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jsp.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vjq.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lrr.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cde.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mon.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://skv.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ppx.zhengqikj.top

================================================================================
来源：http://ehf.nwbrower.top

K. JSON 与序列化
来源：http://wdx.yj20258.top

================================================================================
来源：http://ost.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://vbu.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cmz.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dio.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://oaf.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://zle.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tsu.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://vmz.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://jhg.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zpj.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://thy.52xcode.cn

Py:   json.loads(s)
来源：http://qsw.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ulx.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://phd.gzhubu.top

TS:   JSON.parse(s)
来源：http://oay.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fkv.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://oee.nwbrower.top

Ruby: JSON.parse(s)
来源：http://ohe.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://svp.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://lug.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://foj.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xcv.sjlbkw.cn


<!-- 参考信息 -->