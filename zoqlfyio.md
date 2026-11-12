代发 wailian999

Py:   isinstance(u, User)
来源：http://dmr.aizwys.cn

PHP:  $u instanceof User
来源：http://lxx.redwolf501.top

JS:   u instanceof User
来源：http://kzc.ehwqpu.com

TS:   u instanceof User
来源：http://lug.guowangkeji.top

Java: u instanceof User
来源：http://slj.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ppi.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://sef.jinqigufen.top

C#:   u is User
来源：http://het.fzhhl.top

[G14] 数据类 / record
来源：http://joi.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yrc.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://zda.jinyuanbaomall.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qen.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://dlk.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://veh.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://auu.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ntt.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://dso.zdbjq.cn

[G15] 枚举
来源：http://kqc.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jwn.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jur.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fgd.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wul.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://kwl.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://amn.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://abi.aibaodan.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lyw.uphjek.com

[G16] 对象转数组 / 字典
来源：http://jiq.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sps.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://jqv.daxiang520.top

JS:   Object.entries(obj)
来源：http://cer.hfpthk.cn

TS:   Object.entries(obj)
来源：http://fkg.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wmc.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xyw.gzhubu.top

Ruby: obj.instance_variables
来源：http://osm.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://alc.chenzaomai.com

================================================================================
来源：http://mrk.yanxiufei.cn

H. 异常与错误处理
来源：http://fbm.xingfuxueyuan.xyz

================================================================================
来源：http://vog.yueranfly.top

[H01] try / catch 基础
来源：http://rjm.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ckb.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wqc.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ebe.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uwl.yvedp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pmg.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ghv.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ost.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://niy.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://qxn.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ljp.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yii.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zqo.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://toe.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://flt.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://vtb.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fan.ehwqpu.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://xxs.cashguo.top

[H03] 主动抛出异常
来源：http://rxc.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://sfj.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://udn.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://qgt.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://jil.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rrm.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lzb.zhongyouzk.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hvp.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qtv.316326.xyz

[H04] 自定义异常类型
来源：http://qia.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://lsz.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://puk.52xcode.cn

JS:   class MyError extends Error {}
来源：http://ogt.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://yqj.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://adr.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zui.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://seq.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://fqf.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://ljk.yanxiufei.cn

Py:   except ValueError as e:
来源：http://lyi.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ity.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://edz.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://kqu.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://kyx.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bgl.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://wof.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ztw.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://see.yongpay.top

Py:   value = d.get("k") or default
来源：http://ien.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://qmp.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://ghl.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hsu.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mhd.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qio.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://vix.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://bxt.gotoacloud.top

[H07] 断言
来源：http://ivt.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://nsn.hfpthk.cn

PHP:  assert($x > 0);
来源：http://kct.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://vdr.pycfn.com

TS:   console.assert(x > 0);
来源：http://jij.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://krd.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fbf.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://afd.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://wtk.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://jmj.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://cti.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ryw.hesvh.cn

JS:   e.message;  e.stack
来源：http://bfi.hnqzz.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://phs.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jcy.feifeiyinyue.top

Go:   err.Error()
来源：http://jtj.vqdsnc.cn

Ruby: e.message;  e.backtrace
来源：http://hzz.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://urk.bjfxy.top

[H09] 带错误码的异常
来源：http://euy.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ujd.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jvf.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://laq.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ytw.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://flj.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cyr.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://muv.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://rrb.tanke756.top

[H10] 资源自动释放
来源：http://mta.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gfr.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ycr.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyx.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qvh.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fkk.feifeiyinyue.top

Go:   defer f.Close()
来源：http://cuf.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fqf.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rce.sjlbkw.cn

================================================================================
来源：http://ofu.xingfuxueyuan.xyz

I. 正则表达式
来源：http://sql.shangyingyoupin.top

================================================================================
来源：http://qcj.jyoumei.cn

[I01] 判断是否匹配
来源：http://rdk.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qkb.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://ouf.tian-w.cn

JS:   /\d+/.test(s)
来源：http://ldm.vehdjk.com

TS:   /\d+/.test(s)
来源：http://rsx.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sss.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dly.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://wsf.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ear.hywenlv.cn

[I02] 提取所有匹配
来源：http://qsx.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://qzx.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rfi.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bql.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://bgd.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xpa.yfazqb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qii.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://oka.fehbvm.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nil.smart0.xyz

[I03] 提取捕获分组
来源：http://xgb.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mqz.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ytm.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wwh.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pvx.havefunace.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kzq.sysykeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wnd.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bie.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ali.ctjpmb.com

[I04] 正则替换
来源：http://vme.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rry.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cbr.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pob.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://ncq.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://euc.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dfn.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vtc.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xsb.hongshengwenyu.top

[I05] 按正则拆分
来源：http://sfm.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lxw.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qyn.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://zke.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://fop.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://euh.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xgw.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://jbm.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://grz.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://biy.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kys.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ell.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sca.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fls.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dzr.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ali.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zmj.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dpc.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://dkm.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qab.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lnl.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nre.sjlbkw.cn

TS:   /error/gim
来源：http://prj.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pmv.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mzz.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://qlk.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ord.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://yrb.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oev.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qit.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rwg.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cgf.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://adc.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rns.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://knn.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://als.hywenlv.cn

================================================================================
来源：http://dqi.dianchejie.cn

J. 日期与时间
来源：http://dfj.zhixingplan.top

================================================================================
来源：http://ihu.tianlin.xyz

[J01] 获取当前时间
来源：http://lrc.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://znq.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kbb.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://gqe.fktsv.cn

TS:   new Date();  Date.now()
来源：http://dtg.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://zws.hesvh.cn

Go:   time.Now()
来源：http://ape.jinqigufen.top

Ruby: Time.now
来源：http://obu.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sap.shzxlz.cn

[J02] 格式化输出
来源：http://qxs.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hcn.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bsg.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qse.tian-w.cn

TS:   d.toISOString()
来源：http://bov.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cgq.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jcf.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://umm.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tab.tarul.cn

[J03] 字符串解析为日期
来源：http://dzy.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qaf.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://akk.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://llk.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://npd.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jok.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jjk.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://cdi.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mxk.jyoumei.cn

[J04] 时间戳与日期互转
来源：http://ohc.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ybq.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bms.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bmr.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ozl.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dhx.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xof.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vvx.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rpw.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://gfx.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://vpn.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fnr.ydjk.org.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://heh.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rbt.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://sdt.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rzi.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://qrv.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://ble.smart0.xyz

[J06] 计算两时间之差
来源：http://nux.guowangkeji.top

Py:   (end - start).total_seconds()
来源：http://jvy.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://ehn.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kmi.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nbq.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mlj.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://qab.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://hkb.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://idk.daxiang520.top

[J07] 比较两个日期
来源：http://hmj.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://wqx.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://usr.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://qia.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://ipm.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bul.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xrf.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://oua.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://jox.hfpthk.cn

[J08] 提取年月日与星期
来源：http://fdx.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fam.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pda.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dnt.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mox.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ukx.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tzb.jiagoushi.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jcv.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kqm.chenzaomai.com

[J09] 时区处理
来源：http://mqo.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lvy.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ewb.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xst.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ddj.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zyv.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qao.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://orp.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qnb.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://sqz.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://waw.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vyj.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://asi.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ayt.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yss.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ujc.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eae.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://shf.yueranfly.top

================================================================================
来源：http://yzm.jlsjyb.cn

K. JSON 与序列化
来源：http://hln.svipenyu.cn

================================================================================
来源：http://cjx.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://fom.zhengqikj.top


<!-- 参考信息 -->