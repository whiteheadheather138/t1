代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://xcg.svipenyu.cn

Ruby: def to_s; @name; end
来源：http://eja.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://vno.yanxiufei.cn

[G13] 判断对象类型
来源：http://hvv.9152youxi.cn

Py:   isinstance(u, User)
来源：http://mix.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://ulc.hesvh.cn

JS:   u instanceof User
来源：http://atv.zhengqikj.top

TS:   u instanceof User
来源：http://jxf.wangshuangyany.cn

Java: u instanceof User
来源：http://eki.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eti.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://ylk.chenjidiqi.icu

C#:   u is User
来源：http://oqv.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://pdm.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://edr.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://kme.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://vfu.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://jjf.hcnkem.com

Java: record User(String name, int age) {}
来源：http://ogj.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://niw.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vpd.birdmap.top

C#:   record User(string Name, int Age);
来源：http://wfs.nanxuanxn.top

[G15] 枚举
来源：http://bjd.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nkh.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xyc.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ykt.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bnl.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://zqs.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eqx.jiagoushi.top

Ruby: Color = %i[red green].freeze
来源：http://cna.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sdc.sweek.top

[G16] 对象转数组 / 字典
来源：http://lfr.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kts.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://pbr.xylfe.cn

JS:   Object.entries(obj)
来源：http://wvm.jinyuanbaomall.cn

TS:   Object.entries(obj)
来源：http://opy.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tpf.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ets.chenlongwang.top

Ruby: obj.instance_variables
来源：http://row.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://epc.shangyingyoupin.top

================================================================================
来源：http://jrm.aibaodan.cn

H. 异常与错误处理
来源：http://kqi.c1oappe.top

================================================================================
来源：http://fjl.sjlbkw.cn

[H01] try / catch 基础
来源：http://nas.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bbl.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jsc.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aaq.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lyv.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://set.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gjt.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nkx.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ufn.xuanzx.com

[H02] finally / ensure 收尾
来源：http://clz.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://bdn.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xim.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lpd.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zay.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://czv.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mih.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uao.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ggf.epnwcf.com

[H03] 主动抛出异常
来源：http://bzx.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://whi.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ybx.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://lre.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://gyw.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://him.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://inv.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zpt.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://eex.zhongyouzk.top

[H04] 自定义异常类型
来源：http://rhz.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://sna.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://gbm.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://suy.ybcxt.top

TS:   class MyError extends Error {}
来源：http://okv.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://jhg.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xns.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://xtd.redwolf501.top

C#:   class MyException : Exception {}
来源：http://vaj.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://hnv.nanxinkj.top

Py:   except ValueError as e:
来源：http://ckb.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iwu.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://rbe.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://jfo.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://fkr.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zsa.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://ijm.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kqd.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://odh.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://qaq.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://gse.ydzc1.top

JS:   obj?.a?.b;  d ?? default
来源：http://xui.shzxlz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://akl.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ixi.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vuo.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://yra.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://inj.shanyushiyangkeji.top

[H07] 断言
来源：http://zts.chenjidiqi.icu

Py:   assert x > 0, "必须为正"
来源：http://eas.cucudq.cn

PHP:  assert($x > 0);
来源：http://uhu.cashguo.top

JS:   console.assert(x > 0);
来源：http://kkm.tanke756.top

TS:   console.assert(x > 0);
来源：http://nsj.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://kai.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gpi.zhongyouzk.top

Ruby: raise "必须为正" unless x > 0
来源：http://hor.ivvv.top

C#:   Debug.Assert(x > 0);
来源：http://amu.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://pwj.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://vne.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://abb.316326.xyz

JS:   e.message;  e.stack
来源：http://esf.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pil.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tdl.nanxuanxn.top

Go:   err.Error()
来源：http://acn.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://khj.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://mdv.xuanzx.com

[H09] 带错误码的异常
来源：http://jro.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nju.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eun.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ztm.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dax.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lyk.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fgx.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://hhn.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kgy.zycfv.cn

[H10] 资源自动释放
来源：http://wqz.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wgh.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vpp.cashguo.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ich.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ebj.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uoh.sjlbkw.cn

Go:   defer f.Close()
来源：http://igf.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://opg.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qrh.zhiwuduotai.top

================================================================================
来源：http://vrz.tianlin.xyz

I. 正则表达式
来源：http://hzr.fktsv.cn

================================================================================
来源：http://eia.fzhhl.top

[I01] 判断是否匹配
来源：http://lfs.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nlx.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://fsx.iojbl.cn

JS:   /\d+/.test(s)
来源：http://mky.snrcjt.cn

TS:   /\d+/.test(s)
来源：http://rcm.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jrh.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gqr.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://emy.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zde.andypj.xyz

[I02] 提取所有匹配
来源：http://rod.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://kzz.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bdc.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bbr.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://lop.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iyu.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cev.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://mdj.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tvq.jyoumei.cn

[I03] 提取捕获分组
来源：http://bes.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pji.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pqy.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ewp.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mre.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lxc.guannengcc.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pkn.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ogj.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xtc.jianghu66.top

[I04] 正则替换
来源：http://vzj.chenjidiqi.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://ann.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lsh.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vlc.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vtd.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://zhk.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pkz.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dkf.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://btd.zhiwuduotai.top

[I05] 按正则拆分
来源：http://yfp.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sph.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zyb.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://bpw.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://qkw.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://bmv.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://shq.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://eap.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fzk.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uky.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nhj.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fys.sysykeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://seh.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://niz.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gcg.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iki.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://snu.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yky.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://erb.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gus.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qmd.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ari.jianghu66.top

TS:   /error/gim
来源：http://ssh.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://odz.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lmt.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://nxi.quarkkingdee.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qyb.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://ujx.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pua.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yhy.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qbm.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eca.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yms.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://txt.shanyushiyangtech.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oqp.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://icw.havefunace.top

================================================================================
来源：http://zkm.yuanzhike.top

J. 日期与时间
来源：http://eor.gotoacloud.top

================================================================================
来源：http://ohm.cqqwz.cn

[J01] 获取当前时间
来源：http://jpv.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bcf.guannengcc.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qmq.xylfe.cn

JS:   new Date();  Date.now()
来源：http://ycf.sweek.top

TS:   new Date();  Date.now()
来源：http://dpb.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fyy.yanxiufei.cn

Go:   time.Now()
来源：http://ork.sweek.top

Ruby: Time.now
来源：http://uru.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tye.jinghuilouyu.cn

[J02] 格式化输出
来源：http://ufo.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tui.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mpe.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iss.vqdsnc.cn

TS:   d.toISOString()
来源：http://mtv.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://esr.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gdx.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avx.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pwz.52xcode.cn

[J03] 字符串解析为日期
来源：http://kme.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bmb.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://plq.jinyuanbaomall.cn

JS:   new Date("2024-01-02")
来源：http://ihl.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://cwo.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://lgl.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ihn.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://yer.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kzf.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://obs.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lew.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dws.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fca.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pye.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uvb.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://deg.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fji.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oqv.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://hwo.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://dfm.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eti.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rom.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rsl.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://imz.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tjj.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://ksb.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://kuy.jyoumei.cn

[J06] 计算两时间之差
来源：http://zlf.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://fgo.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://rkz.gogol.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xuh.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ken.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://smz.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://yjt.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://rsk.zycfv.cn

C#:   (end - start).TotalSeconds
来源：http://ztw.snrcjt.cn

[J07] 比较两个日期
来源：http://eqn.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://mqy.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pqp.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://lbj.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://dsy.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nkl.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qqq.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://thx.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://xwj.gogol.net.cn

[J08] 提取年月日与星期
来源：http://fvn.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pno.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://otw.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hsl.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kgg.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dwk.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uab.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pwc.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://drz.sjlbkw.cn

[J09] 时区处理
来源：http://yjj.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://olb.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tnw.shanyushiyangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://art.xuanzx.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ufq.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nzs.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://suf.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://lxe.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qke.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://zcm.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rbb.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iiq.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nte.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zzi.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dfv.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qle.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wlk.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pck.chenlongwang.top


<!-- 参考信息 -->