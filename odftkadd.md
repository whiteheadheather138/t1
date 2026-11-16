代发 wailian999

Py:   isinstance(u, User)
来源：http://bui.xuanzx.com

PHP:  $u instanceof User
来源：http://gvf.epnwcf.com

JS:   u instanceof User
来源：http://wrf.uphjek.com

TS:   u instanceof User
来源：http://pls.iojbl.cn

Java: u instanceof User
来源：http://urt.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ahg.bbcook.cn

Ruby: u.is_a?(User)
来源：http://til.tarul.cn

C#:   u is User
来源：http://vqf.bjfxy.top

[G14] 数据类 / record
来源：http://pda.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fvc.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://joq.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://nev.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://tvc.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://seb.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://lym.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ukn.hammf.cn

C#:   record User(string Name, int Age);
来源：http://ioh.zhixingplan.top

[G15] 枚举
来源：http://ymp.xingfuxueyuan.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xtt.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ncw.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uan.yvedp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://muj.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://wrt.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kpv.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://trh.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kit.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://azg.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yjn.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://dqg.aibaodan.cn

JS:   Object.entries(obj)
来源：http://ely.daxiang520.top

TS:   Object.entries(obj)
来源：http://dks.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cfd.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://puj.cdnleiting.top

Ruby: obj.instance_variables
来源：http://bvb.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://pmr.gzhubu.top

================================================================================
来源：http://hbt.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://duw.fengsongda.top

================================================================================
来源：http://yap.jiagoushi.top

[H01] try / catch 基础
来源：http://njl.gogol.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://brz.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://emf.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tut.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://njx.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gdg.shanyushiyangtech.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ise.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yyo.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ssd.ybcxt.top

[H02] finally / ensure 收尾
来源：http://roa.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://adu.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ati.kuanghao11.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nkk.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://guj.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://dht.ctjpmb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://lje.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vnn.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eie.hfpthk.cn

[H03] 主动抛出异常
来源：http://rrn.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://let.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lje.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://qvp.ivvv.top

TS:   throw new Error("错误信息");
来源：http://hyc.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ost.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ytn.yangfankeji.com

Ruby: raise ArgumentError, "错误信息"
来源：http://acg.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cei.shzxlz.cn

[H04] 自定义异常类型
来源：http://cyv.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://gkc.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ceb.redwolf501.top

JS:   class MyError extends Error {}
来源：http://ibi.fengsongda.top

TS:   class MyError extends Error {}
来源：http://rxy.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://urt.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bgq.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://qug.yonumen.top

C#:   class MyException : Exception {}
来源：http://bxx.fzhhl.top

[H05] 捕获特定类型
来源：http://faj.sjlbkw.cn

Py:   except ValueError as e:
来源：http://prl.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bmx.sufxvd.cn

JS:   if (e instanceof TypeError) {}
来源：http://kze.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://shv.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://zxp.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lsd.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://ncb.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rjb.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://iat.redwolf501.top

Py:   value = d.get("k") or default
来源：http://npg.sjlbkw.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rsd.sweek.top

JS:   obj?.a?.b;  d ?? default
来源：http://umw.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://lmm.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cqd.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hfk.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://iou.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://hqs.svipenyu.cn

[H07] 断言
来源：http://avm.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://qye.mhx1999.top

PHP:  assert($x > 0);
来源：http://mwu.sweek.top

JS:   console.assert(x > 0);
来源：http://arx.wangdashe.top

TS:   console.assert(x > 0);
来源：http://zxd.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://mwv.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pvs.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://bbs.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://kfe.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://jie.gaohongyu789.top

Py:   str(e);  traceback.format_exc()
来源：http://adw.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pek.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://cnz.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://bco.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fzn.zhengqikj.top

Go:   err.Error()
来源：http://ipm.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://oxg.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://cnh.sweek.top

[H09] 带错误码的异常
来源：http://vsh.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dul.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iwo.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rgt.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ops.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://olh.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ore.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://iav.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wna.jqgfzy.top

[H10] 资源自动释放
来源：http://npx.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cdt.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rdc.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://npm.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gbi.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ued.ppjwa.cn

Go:   defer f.Close()
来源：http://nim.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hee.jinqigfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nfd.yfazqb.com

================================================================================
来源：http://dcp.316326.xyz

I. 正则表达式
来源：http://sth.andypj.xyz

================================================================================
来源：http://hro.nwbrower.top

[I01] 判断是否匹配
来源：http://wxq.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tyz.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lot.vehdjk.com

JS:   /\d+/.test(s)
来源：http://osd.fktsv.cn

TS:   /\d+/.test(s)
来源：http://aaw.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tdn.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hhr.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://bxz.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://znr.316326.xyz

[I02] 提取所有匹配
来源：http://gwb.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://gef.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://clm.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xcp.yvedp.cn

TS:   s.match(/\d+/g)
来源：http://snt.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sfe.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ire.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://pvh.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xax.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://oxq.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lxg.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wso.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wnw.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kxv.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sgm.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://flc.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xjx.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jqt.jinyuanbaomall.cn

[I04] 正则替换
来源：http://dih.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://crj.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tyi.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mez.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://wer.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://msk.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://alk.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://olf.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://olo.havefunace.top

[I05] 按正则拆分
来源：http://kpk.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jff.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gez.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://dwn.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://mpk.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://akj.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kki.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://try.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qni.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vas.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cso.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jhz.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fpc.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wbd.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qzv.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gko.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pkk.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://plr.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://kzc.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uty.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ccs.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ukx.ppjwa.cn

TS:   /error/gim
来源：http://wse.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://orj.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yuv.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://vmb.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://peb.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://jeu.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yrj.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rvd.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hni.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gaf.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uow.jlsjyb.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ace.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://enp.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ski.ydjk.org.cn

================================================================================
来源：http://ssn.birdmap.top

J. 日期与时间
来源：http://gmt.gotoacloud.top

================================================================================
来源：http://jcb.nanxuanxn.top

[J01] 获取当前时间
来源：http://dzt.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ypx.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mqy.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://ehf.daxiang520.top

TS:   new Date();  Date.now()
来源：http://mvr.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cky.pycfn.com

Go:   time.Now()
来源：http://xit.shuidangran.top

Ruby: Time.now
来源：http://ygx.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xuc.yuxming.cn

[J02] 格式化输出
来源：http://uim.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rtl.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yfa.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cfr.ydzc1.top

TS:   d.toISOString()
来源：http://ptb.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qpa.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://epl.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mit.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://knx.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://pla.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wcz.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zlw.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://cko.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://fhr.hcnkem.com

Java: LocalDate.parse("2024-01-02")
来源：http://iwt.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cpm.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://svn.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tpg.shuidangran.top

[J04] 时间戳与日期互转
来源：http://cim.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vrr.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fox.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qvm.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://wdt.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sqj.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nkq.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://von.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nnl.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://jad.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://jxs.yongpay.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tqh.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://axr.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zho.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://uhb.xingfuxueyuan.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eyq.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://hyc.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://ykv.snrcjt.cn

[J06] 计算两时间之差
来源：http://nsk.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://dqj.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://kzr.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://okp.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xha.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://xpy.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://kob.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://mya.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://ivo.shuidangran.top

[J07] 比较两个日期
来源：http://lxb.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://ygb.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qlv.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://faw.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://zeb.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zjo.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tsc.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ykl.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://jzq.zdbjq.cn

[J08] 提取年月日与星期
来源：http://jma.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dmy.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gbn.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rxl.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nhw.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://whu.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nlq.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ofb.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gcz.chenlongwang.top

[J09] 时区处理
来源：http://auw.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pal.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ozr.vqdsnc.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://naw.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ell.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://euq.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hbc.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://xdl.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vzb.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://emw.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vzw.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gxm.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://osz.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xet.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lax.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://omd.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tok.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pxd.ybcxt.top

================================================================================
来源：http://dba.hesvh.cn

K. JSON 与序列化
来源：http://aml.iojbl.cn

================================================================================
来源：http://yxz.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://zzk.jqgufenzy.top


<!-- 参考信息 -->