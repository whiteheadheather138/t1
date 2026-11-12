代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://caf.ydjk.org.cn

Ruby: def to_s; @name; end
来源：http://bxi.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://aej.gogol.net.cn

[G13] 判断对象类型
来源：http://grl.0kj1m.cn

Py:   isinstance(u, User)
来源：http://scr.epnwcf.com

PHP:  $u instanceof User
来源：http://duw.zhixingplan.top

JS:   u instanceof User
来源：http://qcy.hesvh.cn

TS:   u instanceof User
来源：http://sdk.wangshuangyany.cn

Java: u instanceof User
来源：http://eoc.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ziv.yueranfly.top

Ruby: u.is_a?(User)
来源：http://nyc.cashguo.top

C#:   u is User
来源：http://eqy.zhengqikj.top

[G14] 数据类 / record
来源：http://lcv.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bkv.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://ywv.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gye.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://zkj.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://wmk.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://esg.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qkc.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://ydv.nanxinkj.top

[G15] 枚举
来源：http://tjk.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rkl.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gcp.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mha.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xng.epnwcf.com

Java: enum Color { RED, GREEN }
来源：http://hdl.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hal.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://xkm.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://umj.fanxiaobao.xyz

[G16] 对象转数组 / 字典
来源：http://pqv.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qka.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://gxg.shzxlz.cn

JS:   Object.entries(obj)
来源：http://qki.epnwcf.com

TS:   Object.entries(obj)
来源：http://mpr.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://anl.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qpx.yj20258888.top

Ruby: obj.instance_variables
来源：http://rjb.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://sgo.vehdjk.com

================================================================================
来源：http://agt.iojbl.cn

H. 异常与错误处理
来源：http://hwd.daria6918.cn

================================================================================
来源：http://xwr.pengpengdd.cyou

[H01] try / catch 基础
来源：http://lpe.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://val.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lxv.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kij.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pdz.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ibm.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ypr.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://htu.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://clz.daxiang520.top

[H02] finally / ensure 收尾
来源：http://vdm.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://don.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://frx.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://zcc.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mis.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://mjy.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cpg.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zbo.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sth.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://vlv.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://wir.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mog.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://trj.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://dlc.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pzj.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lpg.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://exy.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://bcv.zdqjudy.top

[H04] 自定义异常类型
来源：http://qyh.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://asf.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://oxl.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://zbg.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://lji.sweek.top

Java: class MyException extends RuntimeException {}
来源：http://tzk.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kxq.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://tcm.cheryme.top

C#:   class MyException : Exception {}
来源：http://rcj.hnxiangtu.top

[H05] 捕获特定类型
来源：http://mdg.hfpthk.cn

Py:   except ValueError as e:
来源：http://iom.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fbv.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://qvk.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://hse.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://eup.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hjw.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://aoh.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wnp.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://aqr.meibo888.top

Py:   value = d.get("k") or default
来源：http://pyk.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jrj.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://zza.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://tyt.nanxuanxn.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wae.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pwe.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://otr.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://jci.guannengcc.top

[H07] 断言
来源：http://ybi.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://cve.tanke756.top

PHP:  assert($x > 0);
来源：http://yzs.gzhubu.top

JS:   console.assert(x > 0);
来源：http://nue.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://ird.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://kwi.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uqd.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://vcv.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://oov.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://bdi.jianghu66.top

Py:   str(e);  traceback.format_exc()
来源：http://rro.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://acj.havefunace.top

JS:   e.message;  e.stack
来源：http://vik.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://naa.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://uov.feifeiyinyue.top

Go:   err.Error()
来源：http://qcf.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://utu.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://skj.uphjek.com

[H09] 带错误码的异常
来源：http://hln.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yqj.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dsc.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fqk.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://krg.havefunace.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kag.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://edk.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://dny.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wqh.wangshuangyany.cn

[H10] 资源自动释放
来源：http://mpy.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://azs.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ueq.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://smt.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wsb.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jep.cucudq.cn

Go:   defer f.Close()
来源：http://ctd.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eyh.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipp.chenjidiqi.icu

================================================================================
来源：http://zvl.zhixingplan.top

I. 正则表达式
来源：http://jru.meibo888.top

================================================================================
来源：http://rob.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://jll.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vws.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uaq.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://gcd.yj20258888.top

TS:   /\d+/.test(s)
来源：http://czs.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wzu.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jgt.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://svk.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://juu.cashguo.top

[I02] 提取所有匹配
来源：http://nfj.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://ekk.gotoacloud.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://upt.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fms.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://omc.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bkn.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://soq.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://swk.yuanzhike.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rvq.chenlongwang.top

[I03] 提取捕获分组
来源：http://zpv.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fmk.chenzaomai.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vsg.hesvh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://brg.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://moc.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://afp.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rbt.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fxy.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://asp.nanxinkj.top

[I04] 正则替换
来源：http://aij.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jom.jianghu66.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xla.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://ytr.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://wym.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://ehr.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cjs.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vqr.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mpy.yuxming.cn

[I05] 按正则拆分
来源：http://udw.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wuy.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rge.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://rvw.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://shi.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://gal.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hvi.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://wqm.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xhk.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kfn.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iwk.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qhp.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtj.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mnd.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://let.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://goz.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cwa.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hbx.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://squ.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://keh.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ukt.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://asj.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://hxn.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dax.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cnu.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://kvl.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nfz.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://wgw.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rzi.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dvi.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zig.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfs.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gdz.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ygy.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rif.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lkt.ehwqpu.com

================================================================================
来源：http://yta.wangdashe.top

J. 日期与时间
来源：http://nfk.xziqi.cn

================================================================================
来源：http://gpx.svipenyu.cn

[J01] 获取当前时间
来源：http://gdy.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://edp.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bnc.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://ajf.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://uvi.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fzn.shangyingyoupin.top

Go:   time.Now()
来源：http://ppj.cheryme.top

Ruby: Time.now
来源：http://qtn.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mnb.zhiwuduotai.top

[J02] 格式化输出
来源：http://uin.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwv.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aup.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://htm.yj20258.top

TS:   d.toISOString()
来源：http://cnq.zhaomingkeji.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eaj.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zzi.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbm.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uvk.wangdashe.top

[J03] 字符串解析为日期
来源：http://ywk.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vmo.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rde.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://zby.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://oeb.fengsongda.top

Java: LocalDate.parse("2024-01-02")
来源：http://tgk.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hbk.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://jag.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rer.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://ytu.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qvz.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iia.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qls.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://qqp.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://spz.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://msh.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vvb.chenzaomai.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qgd.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://pvy.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://bok.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eoe.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tpe.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zhf.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://rvj.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://teo.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://zpl.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://cjg.chenzaomai.com

[J06] 计算两时间之差
来源：http://jls.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://qdu.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://qug.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mza.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fzp.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://qlc.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://tba.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://jcl.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://pol.mhx1999.top

[J07] 比较两个日期
来源：http://qph.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://qzt.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vqd.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://aom.nanxuanxn.top

TS:   d1.getTime() < d2.getTime()
来源：http://dqv.jqgfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ckf.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lsi.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lej.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://qvx.uphjek.com

[J08] 提取年月日与星期
来源：http://xto.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xon.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yjh.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pek.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uez.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tje.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ilo.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dxf.tianlin.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pcp.hfpthk.cn

[J09] 时区处理
来源：http://fnn.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rsw.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xmf.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zll.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vlx.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iod.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hrl.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://def.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zse.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://kpw.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oct.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://njl.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ayf.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kee.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gpn.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tvc.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wgr.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wgr.redwolf501.top


<!-- 参考信息 -->