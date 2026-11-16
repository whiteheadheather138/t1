代发 wailian999

[G14] 数据类 / record
来源：http://qtx.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mip.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://rae.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://aio.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://dlo.yj202588.top

Java: record User(String name, int age) {}
来源：http://grg.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://dym.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://avv.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://mmk.kuanghao11.cn

[G15] 枚举
来源：http://mlg.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vol.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lmd.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sor.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qkk.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://svu.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qmx.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://pdz.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vxe.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://enz.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jpr.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://zfi.ivvv.top

JS:   Object.entries(obj)
来源：http://qek.ivvv.top

TS:   Object.entries(obj)
来源：http://cmb.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vyn.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bgk.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://dgj.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://jub.yuxming.cn

================================================================================
来源：http://hub.jinqigfzy.top

H. 异常与错误处理
来源：http://cbz.xuetiantiany.cn

================================================================================
来源：http://hgo.jqgfzy.top

[H01] try / catch 基础
来源：http://blq.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ecj.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qef.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://twk.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lij.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://psv.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cie.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sbq.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uly.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://apo.birdmap.top

Py:   try: f()⏎finally: cleanup()
来源：http://ivh.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dsu.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://agq.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qgy.vehdjk.com

Java: try { f(); } finally { cleanup(); }
来源：http://tzn.nanxinkj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ojr.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://moc.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://urm.gaohongyu789.top

[H03] 主动抛出异常
来源：http://yps.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://eky.quarkkingdee.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rmk.yj20258.top

JS:   throw new Error("错误信息");
来源：http://twk.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://fzw.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ibo.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tpa.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zth.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://brd.ppjwa.cn

[H04] 自定义异常类型
来源：http://kwn.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://qlu.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zie.fehbvm.com

JS:   class MyError extends Error {}
来源：http://uhh.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://yet.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://zxo.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qrd.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://myw.fengsongda.top

C#:   class MyException : Exception {}
来源：http://sik.nanxuanxn.top

[H05] 捕获特定类型
来源：http://vuy.daria6918.cn

Py:   except ValueError as e:
来源：http://imw.fzhhl.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gxg.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://pyg.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://bfy.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://yav.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vgq.nanxuanxn.top

Ruby: rescue ArgumentError => e
来源：http://rgj.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ven.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://hio.yvedp.cn

Py:   value = d.get("k") or default
来源：http://mui.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://hjc.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://nhi.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://rlq.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cvv.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pxo.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://sow.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://ivt.hnqzz.top

[H07] 断言
来源：http://dof.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://ebm.nanxinkj.top

PHP:  assert($x > 0);
来源：http://oln.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://pps.yj202588.top

TS:   console.assert(x > 0);
来源：http://kwd.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://fbg.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dje.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://keu.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://qwg.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://hte.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://djy.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dke.zhengqikj.top

JS:   e.message;  e.stack
来源：http://nod.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://yzn.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pfa.fktsv.cn

Go:   err.Error()
来源：http://zat.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://lim.snrcjt.cn

C#:   e.Message;  e.StackTrace
来源：http://upi.daxiang520.top

[H09] 带错误码的异常
来源：http://lcc.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ujn.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jaf.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ahs.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zpe.jinyuanbaomall.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://prg.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xtz.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://kzm.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://yuw.shuidangran.top

[H10] 资源自动释放
来源：http://swp.wangdashe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gfm.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sfu.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ihi.zdbjq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bai.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pti.yuanzhike.top

Go:   defer f.Close()
来源：http://zpo.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://raw.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ivr.chenjidiqi.icu

================================================================================
来源：http://djp.uphjek.com

I. 正则表达式
来源：http://bjx.fzhhl.top

================================================================================
来源：http://cas.fzhhl.top

[I01] 判断是否匹配
来源：http://yqk.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oag.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://kma.fzhhl.top

JS:   /\d+/.test(s)
来源：http://csz.fktsv.cn

TS:   /\d+/.test(s)
来源：http://qpg.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://swv.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ytt.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://wsi.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qud.ydjk.org.cn

[I02] 提取所有匹配
来源：http://qbi.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://fsm.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xtf.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rtx.birdmap.top

TS:   s.match(/\d+/g)
来源：http://tad.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rih.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lts.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://gby.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hlm.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://szf.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jsh.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eql.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ucw.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vnk.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jch.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://res.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://utk.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://epp.hcnkem.com

[I04] 正则替换
来源：http://obl.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qha.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpb.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://ems.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://lqa.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://hse.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bfh.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://cpz.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ume.snrcjt.cn

[I05] 按正则拆分
来源：http://cnx.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wuf.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gng.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://ncz.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://bed.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://sxz.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cps.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://xub.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://grb.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ilz.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdn.gotoacloud.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qra.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://stf.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqe.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tdk.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tct.snrcjt.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ifg.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mjs.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://mzj.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lde.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vxr.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dsh.hesvh.cn

TS:   /error/gim
来源：http://snn.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wud.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vdl.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://ncz.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nhc.jinqigufen.top

[I08] 贪婪与非贪婪匹配
来源：http://tby.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hxi.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gig.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ukm.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aho.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sga.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xpk.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kay.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qms.xingfuxueyuan.xyz

================================================================================
来源：http://aqo.zhijiandao.cn

J. 日期与时间
来源：http://hrc.hongshengwenyu.top

================================================================================
来源：http://xsf.aibaodan.cn

[J01] 获取当前时间
来源：http://mdx.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yie.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ibc.daxiang520.top

JS:   new Date();  Date.now()
来源：http://ojh.fehbvm.com

TS:   new Date();  Date.now()
来源：http://wwq.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fya.cheryme.top

Go:   time.Now()
来源：http://eaz.zycfv.cn

Ruby: Time.now
来源：http://nkx.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lir.9152youxi.cn

[J02] 格式化输出
来源：http://rrz.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://afd.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dlh.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fxc.cashguo.top

TS:   d.toISOString()
来源：http://vep.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yqo.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://snb.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ouv.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://enq.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://yau.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vtb.hcnkem.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qyd.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://mcx.zhongyouzk.top

TS:   new Date("2024-01-02")
来源：http://ozb.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gaq.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rwf.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://osm.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wer.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://kcw.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vvk.hesvh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xtk.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lge.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ihx.haohaochexian.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yrf.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://far.xuetiantiany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ntv.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://itg.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://mny.zhijiandao.cn

Py:   now + timedelta(days=7)
来源：http://rrb.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pnv.xylfe.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://scj.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://umz.ppjwa.cn

Java: LocalDate.now().plusDays(7)
来源：http://xpx.gogol.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jkf.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://ggf.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vql.sweek.top

[J06] 计算两时间之差
来源：http://nlb.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://xvg.yuanzhike.top

PHP:  $end->diff($start)->days;
来源：http://roq.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wcf.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vjh.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ifd.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://txr.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://cfk.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://bvd.fzhhl.top

[J07] 比较两个日期
来源：http://ayw.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://csw.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://puo.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://hno.dianchejie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jez.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oxd.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sxz.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://whu.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://krn.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://mxc.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jwg.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nrh.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cce.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aqr.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kpg.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://afc.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rar.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jaa.gzhubu.top

[J09] 时区处理
来源：http://nka.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ilr.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oli.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://elj.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://joy.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rav.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://geu.chenlongwang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sbh.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cwu.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://gtv.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ukd.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uxq.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xsc.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wmf.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://auy.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uzj.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rcw.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jqg.hysaishi.cn

================================================================================
来源：http://oew.nanxuanxn.top

K. JSON 与序列化
来源：http://oil.epnwcf.com

================================================================================
来源：http://mms.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://vza.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cgu.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bhy.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://qfz.uphjek.com

TS:   JSON.stringify(obj)
来源：http://xbf.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rbx.vehdjk.com

Go:   json.Marshal(obj)
来源：http://aql.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://mfv.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://cdo.sjlbkw.cn


<!-- 参考信息 -->