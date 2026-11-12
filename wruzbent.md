代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hns.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://sbs.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://tst.wangshuangyany.cn

[G13] 判断对象类型
来源：http://qpq.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://grv.9152youxi.cn

PHP:  $u instanceof User
来源：http://ntg.zdbjq.cn

JS:   u instanceof User
来源：http://wef.jinqigufen.top

TS:   u instanceof User
来源：http://jqx.nanxinkj.top

Java: u instanceof User
来源：http://dpz.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pby.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://xtf.snrcjt.cn

C#:   u is User
来源：http://eor.zdbjq.cn

[G14] 数据类 / record
来源：http://ids.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sqa.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://xri.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://vun.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://maw.tian-w.cn

Java: record User(String name, int age) {}
来源：http://qsy.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://vfn.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ctm.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://dns.tarul.cn

[G15] 枚举
来源：http://vqq.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gib.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mad.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kdh.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fut.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://lfn.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hgc.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://iql.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vdy.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://mmh.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ajg.yj202588.top

PHP:  get_object_vars($obj);
来源：http://bvz.sysykeji.top

JS:   Object.entries(obj)
来源：http://qip.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://nwh.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wxc.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://oeo.jiagoushi.top

Ruby: obj.instance_variables
来源：http://duy.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://gys.mhx1999.top

================================================================================
来源：http://cgj.kuanghao11.cn

H. 异常与错误处理
来源：http://lfj.xziqi.cn

================================================================================
来源：http://fbp.ydzc1.top

[H01] try / catch 基础
来源：http://aci.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xya.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eva.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qxl.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bvi.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ulj.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kwb.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://npb.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fyb.zycfv.cn

[H02] finally / ensure 收尾
来源：http://ckl.shzxlz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vjk.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qyr.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://clm.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wjp.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hfl.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uhu.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://htc.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gke.snrcjt.cn

[H03] 主动抛出异常
来源：http://apy.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://ijj.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cnt.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://rvk.yangfankeji.com

TS:   throw new Error("错误信息");
来源：http://yhs.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ahh.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://obq.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://spb.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://qpj.pycfn.com

[H04] 自定义异常类型
来源：http://rin.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://cbs.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://axq.uphjek.com

JS:   class MyError extends Error {}
来源：http://fyk.andypj.xyz

TS:   class MyError extends Error {}
来源：http://eic.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://vjr.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zfm.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://qff.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://qyq.sysykeji.top

[H05] 捕获特定类型
来源：http://sar.jlsjyb.cn

Py:   except ValueError as e:
来源：http://rgl.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pku.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://ate.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://qhq.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://kic.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gkv.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://dba.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kyu.cashguo.top

[H06] 可选值 / 空值安全访问
来源：http://trr.cheryme.top

Py:   value = d.get("k") or default
来源：http://ruf.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://euu.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://eee.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://jzb.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nda.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pgk.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://oxr.xziqi.cn

C#:   obj?.A?.B ?? default
来源：http://jsn.shzxlz.cn

[H07] 断言
来源：http://wdt.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://ayh.epnwcf.com

PHP:  assert($x > 0);
来源：http://rdi.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://tgn.iojbl.cn

TS:   console.assert(x > 0);
来源：http://jcd.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://wpz.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://meu.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://cpw.jinyuanbaomall.cn

C#:   Debug.Assert(x > 0);
来源：http://pqt.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://ivf.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://jii.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dek.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://wdf.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://rps.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tiy.aibaodan.cn

Go:   err.Error()
来源：http://oop.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://ryr.zhengqikj.top

C#:   e.Message;  e.StackTrace
来源：http://wuf.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://gzd.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://urp.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bvb.hnqzz.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bjr.dashuyun.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ujc.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pkl.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kbe.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://szr.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zih.nwbrower.top

[H10] 资源自动释放
来源：http://xxq.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://otk.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lds.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sqh.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hij.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pir.sysykeji.top

Go:   defer f.Close()
来源：http://jaz.yangfankeji.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mid.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bpp.fzhhl.top

================================================================================
来源：http://ayi.xuetiantiany.cn

I. 正则表达式
来源：http://hcj.birdmap.top

================================================================================
来源：http://yku.tarul.cn

[I01] 判断是否匹配
来源：http://ewh.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ced.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yhf.316326.xyz

JS:   /\d+/.test(s)
来源：http://hpz.daria6918.cn

TS:   /\d+/.test(s)
来源：http://trg.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xvc.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ldq.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://uwg.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rpl.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://gcs.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://oke.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://exx.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wbz.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://mue.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://azl.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://prp.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://mwa.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://scm.zdbjq.cn

[I03] 提取捕获分组
来源：http://tgk.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nwc.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uio.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wpi.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pfr.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://opa.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wig.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hsj.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ybq.fktsv.cn

[I04] 正则替换
来源：http://sbi.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zpp.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmh.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://vik.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://rto.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://nso.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tbx.jinyuanbaomall.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xcr.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yvk.aibaodan.cn

[I05] 按正则拆分
来源：http://ymb.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://hcr.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://inn.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://rpx.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://gof.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://auh.jlsjyb.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uff.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://myf.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cvt.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://urj.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ffc.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qcm.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nut.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yta.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ooa.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nwa.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ein.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yob.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://osz.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://phz.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gqn.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zxe.tianlin.xyz

TS:   /error/gim
来源：http://bmt.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pma.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://klc.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://ziu.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ypu.mhx1999.top

[I08] 贪婪与非贪婪匹配
来源：http://usg.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yki.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ymy.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vtd.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oze.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yxl.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wut.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rpp.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dms.wangshuangyany.cn

================================================================================
来源：http://azz.yanxiufei.cn

J. 日期与时间
来源：http://eiq.pycfn.com

================================================================================
来源：http://pew.fzhhl.top

[J01] 获取当前时间
来源：http://vxf.daxiang520.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://izk.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://msl.yj20258888.top

JS:   new Date();  Date.now()
来源：http://zfg.andypj.xyz

TS:   new Date();  Date.now()
来源：http://wns.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sdc.shanyushiyangtech.top

Go:   time.Now()
来源：http://cey.zhoulong.xyz

Ruby: Time.now
来源：http://puq.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fim.yj20258888.top

[J02] 格式化输出
来源：http://kww.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lkg.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rhn.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qts.guannengcc.top

TS:   d.toISOString()
来源：http://xcb.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wjw.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jzt.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cdh.smart0.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://azn.cucudq.cn

[J03] 字符串解析为日期
来源：http://sic.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wvy.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nlz.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://kml.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://bmz.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://rvv.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oiv.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://lji.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dzu.yuxming.cn

[J04] 时间戳与日期互转
来源：http://ayi.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kog.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wke.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fgs.zdqjudy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ikn.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ftr.bbcook.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gkc.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jlg.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://seq.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://nwc.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://rpd.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yxl.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzc.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yuu.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://jyk.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://obu.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://woo.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://pps.quarkkingdee.top

[J06] 计算两时间之差
来源：http://dki.ivvv.top

Py:   (end - start).total_seconds()
来源：http://ota.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://nsp.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://emv.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gro.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ooi.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://wym.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://htn.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://uum.gotoacloud.top

[J07] 比较两个日期
来源：http://epk.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ikt.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dch.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://lpc.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nsg.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ooy.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ytj.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://lhq.0kj1m.cn

C#:   d1 < d2;  d1 == d2
来源：http://onv.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://pmp.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vhp.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kqw.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kse.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kaf.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bum.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vsn.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cqo.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rvk.daria6918.cn

[J09] 时区处理
来源：http://xsl.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ttq.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bgg.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqh.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asn.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dzz.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://roy.pengpengdd.cyou

Ruby: Time.now.getlocal("+08:00")
来源：http://qqj.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://skn.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://xzi.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://alb.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ddc.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yca.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wyd.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://csh.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tai.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://emn.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ozy.52xcode.cn


<!-- 参考信息 -->