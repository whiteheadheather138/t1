代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://ipd.sysykeji.top

Ruby: def to_s; @name; end
来源：http://shx.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://evc.xziqi.cn

[G13] 判断对象类型
来源：http://rls.jianghu66.top

Py:   isinstance(u, User)
来源：http://jtc.ctjpmb.com

PHP:  $u instanceof User
来源：http://okp.jinqigufen.top

JS:   u instanceof User
来源：http://ewf.jqgfzy.top

TS:   u instanceof User
来源：http://uac.birdmap.top

Java: u instanceof User
来源：http://ugw.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qad.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://mnc.xinyue.icu

C#:   u is User
来源：http://izr.yanxiufei.cn

[G14] 数据类 / record
来源：http://ooy.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vij.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://hda.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://cgv.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://vns.birdmap.top

Java: record User(String name, int age) {}
来源：http://kyv.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://trs.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xqb.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://wpy.svipenyu.cn

[G15] 枚举
来源：http://htd.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://srh.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://yit.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kjg.zdbjq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rwc.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://sbk.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jrp.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://kbi.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://myw.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://irb.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lxs.cheryme.top

PHP:  get_object_vars($obj);
来源：http://wvj.yvedp.cn

JS:   Object.entries(obj)
来源：http://xyc.52xcode.cn

TS:   Object.entries(obj)
来源：http://mfa.aizwys.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://saf.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://weq.birdmap.top

Ruby: obj.instance_variables
来源：http://wks.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://drm.shanyushiyangtech.top

================================================================================
来源：http://gkj.tianlin.xyz

H. 异常与错误处理
来源：http://buc.nanxuanxn.top

================================================================================
来源：http://boe.zycfv.cn

[H01] try / catch 基础
来源：http://wqh.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cer.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vcc.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hyb.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ffs.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cjo.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://maq.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wyk.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nuj.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://yjo.xuanzx.com

Py:   try: f()⏎finally: cleanup()
来源：http://hod.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lie.ivvv.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xhl.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://azf.zhoulong.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ocq.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cwg.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iik.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://anm.yueranfly.top

[H03] 主动抛出异常
来源：http://ben.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://kxi.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iva.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://uxv.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://ewd.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nhe.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://luy.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ssh.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://fbh.ivvv.top

[H04] 自定义异常类型
来源：http://ume.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://ojl.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://hhc.vehdjk.com

JS:   class MyError extends Error {}
来源：http://hgw.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://mmt.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://njd.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lnv.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://ivb.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://kax.fzhhl.top

[H05] 捕获特定类型
来源：http://gyg.jqgfzy.top

Py:   except ValueError as e:
来源：http://hjf.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xfi.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://car.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://xna.pycfn.com

Java: catch (IOException | SQLException e) {}
来源：http://lfg.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wja.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://ffy.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pqn.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://kna.fzhhl.top

Py:   value = d.get("k") or default
来源：http://ehq.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://pwc.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://gyb.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lth.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dfi.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://eez.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://mpd.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://jel.jinyuanbaomall.cn

[H07] 断言
来源：http://vdl.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://tfy.ctjpmb.com

PHP:  assert($x > 0);
来源：http://nmd.xziqi.cn

JS:   console.assert(x > 0);
来源：http://cmi.xziqi.cn

TS:   console.assert(x > 0);
来源：http://wjc.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://owq.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://umf.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dps.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://aon.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://pul.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://xba.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qxr.pycfn.com

JS:   e.message;  e.stack
来源：http://izc.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cpc.fktsv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hfz.tanke756.top

Go:   err.Error()
来源：http://ama.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://rbj.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://pgr.dianchejie.cn

[H09] 带错误码的异常
来源：http://gua.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ipd.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dmk.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dde.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zkh.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://okt.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vku.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gmd.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://sru.yangfankeji.com

[H10] 资源自动释放
来源：http://vnm.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dtd.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ttg.yangfankeji.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mmh.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gsx.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://msk.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://qbg.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uxi.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qqc.52xcode.cn

================================================================================
来源：http://gur.pycfn.com

I. 正则表达式
来源：http://lvd.vehdjk.com

================================================================================
来源：http://tfp.bbcook.cn

[I01] 判断是否匹配
来源：http://jhb.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qgp.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://vlj.daria6918.cn

JS:   /\d+/.test(s)
来源：http://jgr.aizwys.cn

TS:   /\d+/.test(s)
来源：http://pqn.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ved.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qpp.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://tsi.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cnd.jlsjyb.cn

[I02] 提取所有匹配
来源：http://yob.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://dke.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qxc.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lvc.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://mld.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hgq.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ihr.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://olf.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wno.svipenyu.cn

[I03] 提取捕获分组
来源：http://leo.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kkw.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hce.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rda.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://onr.yj20258888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qxn.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://anw.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rio.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pze.zhaomingkeji.xyz

[I04] 正则替换
来源：http://ljw.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vxq.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dnz.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://wsw.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uwg.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://jpa.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qne.jinyuanbaomall.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fge.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lzf.yj20258888.top

[I05] 按正则拆分
来源：http://wil.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yro.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://znk.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://wyz.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://lgj.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://nil.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xfk.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://ygj.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rzz.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nvg.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jis.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sys.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxj.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewj.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gtc.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lzb.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oto.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gat.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://ypl.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fhn.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dfa.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tvp.shuidangran.top

TS:   /error/gim
来源：http://vwp.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yjw.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://upn.yongpay.top

Ruby: s.scan(/error/i)
来源：http://wcw.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jzn.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://iiw.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nyk.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ofv.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqw.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cia.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ald.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ggy.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yhm.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blq.xylfe.cn

================================================================================
来源：http://cjo.yuxming.cn

J. 日期与时间
来源：http://ihc.hcnkem.com

================================================================================
来源：http://ijg.hongshengwenyu.top

[J01] 获取当前时间
来源：http://yns.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ngg.9152youxi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gas.fanxiaobao.xyz

JS:   new Date();  Date.now()
来源：http://afh.iojbl.cn

TS:   new Date();  Date.now()
来源：http://pwv.tian-w.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://myi.fktsv.cn

Go:   time.Now()
来源：http://kst.chenjidiqi.icu

Ruby: Time.now
来源：http://ldv.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mrq.ppjwa.cn

[J02] 格式化输出
来源：http://pyn.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qma.yfazqb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yzg.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pwi.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://hfm.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://its.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bbh.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://njp.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gpp.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://kyn.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ivl.bbcook.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pme.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://bew.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://cly.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zgj.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eqj.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://ieu.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eyb.fktsv.cn

[J04] 时间戳与日期互转
来源：http://sng.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yce.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oyp.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pqb.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ntf.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://swv.yj20258888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mtq.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jth.chenlongwang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xry.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://iww.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://tbf.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gpr.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sls.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yys.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://vyh.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://umh.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://sux.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://beq.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://iig.feifeiyinyue.top

Py:   (end - start).total_seconds()
来源：http://fck.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://wuc.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dkk.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tdl.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ceu.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://cdr.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://nkk.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://kvu.yongpay.top

[J07] 比较两个日期
来源：http://tuf.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://tig.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jwz.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hkp.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://gyq.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ddi.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ocv.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://cxh.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://kmz.sysykeji.top

[J08] 提取年月日与星期
来源：http://yab.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ntq.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wjg.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zar.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rvy.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://abq.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fxe.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fzs.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eyr.shangyingyoupin.top

[J09] 时区处理
来源：http://dfb.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xhe.smart0.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cbe.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fsf.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://icd.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qyv.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rhr.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fnq.jinqigfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://syf.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://jsv.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nws.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jxy.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xln.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://omh.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ecp.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bmm.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hkl.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mof.jyoumei.cn


<!-- 参考信息 -->