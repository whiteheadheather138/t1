代发 wailian999

Java: u instanceof User
来源：http://lpy.jqgufenzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mmf.fzhhl.top

Ruby: u.is_a?(User)
来源：http://gos.ydzc1.top

C#:   u is User
来源：http://ten.yj20258888.top

[G14] 数据类 / record
来源：http://ecq.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gpo.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://kco.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://rkb.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://ogk.316326.xyz

Java: record User(String name, int age) {}
来源：http://ytv.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://ybt.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zhh.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://qgc.cucudq.cn

[G15] 枚举
来源：http://uyh.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mtg.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lly.cdnleiting.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://use.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kcb.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://aat.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eqo.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://alr.tarul.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lxz.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://pfa.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gui.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://yal.epnwcf.com

JS:   Object.entries(obj)
来源：http://zmy.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://bji.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kcz.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tko.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://fft.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://vrh.yueranfly.top

================================================================================
来源：http://jef.ydzc1.top

H. 异常与错误处理
来源：http://tsk.guowangkeji.top

================================================================================
来源：http://qcx.xziqi.cn

[H01] try / catch 基础
来源：http://pyw.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iwp.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://moo.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tva.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fjy.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://csd.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kwd.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://luk.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tqs.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://yiq.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://gea.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ore.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://app.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://die.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://ucv.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://koo.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://opq.hywenlv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gdw.cashguo.top

[H03] 主动抛出异常
来源：http://zms.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://ddu.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ifv.ehwqpu.com

JS:   throw new Error("错误信息");
来源：http://hkm.cashguo.top

TS:   throw new Error("错误信息");
来源：http://evw.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qeu.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qzz.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ast.jinghuilouyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ttw.xziqi.cn

[H04] 自定义异常类型
来源：http://vwg.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://edu.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uan.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://hhe.iojbl.cn

TS:   class MyError extends Error {}
来源：http://agh.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://xfm.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tuq.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://vyf.yvedp.cn

C#:   class MyException : Exception {}
来源：http://clk.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://pum.yj202588.top

Py:   except ValueError as e:
来源：http://awv.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sep.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://loj.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://usl.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://zay.hywenlv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vpv.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://ttk.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dfy.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://hyr.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://yhp.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ajb.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://zoh.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tkd.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bxs.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mop.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://vfp.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://ayo.xingfuxueyuan.xyz

[H07] 断言
来源：http://cpx.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://hac.shzxlz.cn

PHP:  assert($x > 0);
来源：http://evl.pycfn.com

JS:   console.assert(x > 0);
来源：http://rws.xziqi.cn

TS:   console.assert(x > 0);
来源：http://xmt.xuanzx.com

Java: assert x > 0 : "必须为正";
来源：http://hbw.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vqj.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://rgx.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://guv.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://suk.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://vae.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tux.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://mne.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kfr.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mfz.cucudq.cn

Go:   err.Error()
来源：http://qow.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://jmv.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://pql.hcnkem.com

[H09] 带错误码的异常
来源：http://fwl.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kaf.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rvh.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ptq.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kif.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ias.fengsongda.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lde.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qlr.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lwb.hesvh.cn

[H10] 资源自动释放
来源：http://mxh.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ttc.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gns.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ohd.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://amt.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jkb.dianchejie.cn

Go:   defer f.Close()
来源：http://xwq.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ctj.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bdt.yj20258.top

================================================================================
来源：http://wdm.quarkkingdee.top

I. 正则表达式
来源：http://rgb.tanke756.top

================================================================================
来源：http://kkw.ivvv.top

[I01] 判断是否匹配
来源：http://uuc.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ahf.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://nqi.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://wxl.havefunace.top

TS:   /\d+/.test(s)
来源：http://txy.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lwz.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wga.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://zpr.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kes.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://owp.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://pxe.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://avy.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cbe.daria6918.cn

TS:   s.match(/\d+/g)
来源：http://gpl.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iky.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dlr.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://iru.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dqi.yuanzhike.top

[I03] 提取捕获分组
来源：http://vmw.hnxiangtu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vdz.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kgs.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://irm.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kbv.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://anh.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wpt.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xqj.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xzl.cdnleiting.top

[I04] 正则替换
来源：http://hda.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jdb.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mwf.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://mqv.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hqi.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://ixs.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jae.xziqi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://okh.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wka.havefunace.top

[I05] 按正则拆分
来源：http://ntj.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://fmt.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zlv.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://lzi.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://aba.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://tog.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xzm.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://qvz.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://okn.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tta.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kzi.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lim.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sbj.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vuo.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lzb.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jvd.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wox.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://koa.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://mez.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://het.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nyt.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://trc.bbcook.cn

TS:   /error/gim
来源：http://zdp.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kdz.jinyuanbaomall.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://clx.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://zrr.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://snd.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://wed.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fvd.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cfa.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nfr.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ucg.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qtv.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jhu.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://psy.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sid.zycfv.cn

================================================================================
来源：http://pun.pengpengdd.cyou

J. 日期与时间
来源：http://sra.ehwqpu.com

================================================================================
来源：http://osf.hnqzz.top

[J01] 获取当前时间
来源：http://epd.c1oappe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sku.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hfl.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://dmi.mhx1999.top

TS:   new Date();  Date.now()
来源：http://voo.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iii.zycfv.cn

Go:   time.Now()
来源：http://ngx.gogol.net.cn

Ruby: Time.now
来源：http://nlg.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yjz.ivvv.top

[J02] 格式化输出
来源：http://kks.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mau.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ohc.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://okc.0kj1m.cn

TS:   d.toISOString()
来源：http://iyr.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://obs.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blv.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xem.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kbd.dashuyun.cn

[J03] 字符串解析为日期
来源：http://rrm.jinqigfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ave.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qjk.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://her.tanke756.top

TS:   new Date("2024-01-02")
来源：http://ucm.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://ehe.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yzu.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://xeq.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tqs.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://lew.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ijs.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://suw.pengpengdd.cyou

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://trp.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ero.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xzn.ctjpmb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sue.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fbv.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://myt.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://tjr.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://gta.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nex.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zuo.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fdi.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://iub.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://amk.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://equ.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cvw.xuanzx.com

[J06] 计算两时间之差
来源：http://wzk.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://yhc.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://ako.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxi.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yle.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cew.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://jmu.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://ask.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://art.birdmap.top

[J07] 比较两个日期
来源：http://ghi.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://uya.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hxl.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://deb.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://ajh.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://foa.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yga.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://akh.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://rmv.tianlin.xyz

[J08] 提取年月日与星期
来源：http://mfg.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dab.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qip.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dmq.redwolf501.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fgx.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pnc.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xtx.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eho.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jse.pycfn.com

[J09] 时区处理
来源：http://yhe.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mas.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bui.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://isb.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zqc.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lek.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://llv.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pcq.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ycl.yvedp.cn

[J10] 取今天 / 本月第一天
来源：http://rdp.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bbm.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://css.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xtt.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xok.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gub.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ath.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sho.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cun.cqqwz.cn

================================================================================
来源：http://fjw.smart0.xyz

K. JSON 与序列化
来源：http://gjq.hnxiangtu.top

================================================================================
来源：http://mwz.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://rmi.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oen.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zii.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://yor.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://xrv.yj20258.top


<!-- 参考信息 -->