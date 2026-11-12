代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://xdi.mhx1999.top

JS:   toString() { return this.name; }
来源：http://pnb.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://njs.guowangkeji.top

Java: @Override public String toString() { return name; }
来源：http://yty.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://age.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://aak.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://cje.vehdjk.com

[G13] 判断对象类型
来源：http://csj.daria6918.cn

Py:   isinstance(u, User)
来源：http://tda.jqgufenzy.top

PHP:  $u instanceof User
来源：http://ars.yongpay.top

JS:   u instanceof User
来源：http://yor.birdmap.top

TS:   u instanceof User
来源：http://jwp.c1oappe.top

Java: u instanceof User
来源：http://ycg.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mil.havefunace.top

Ruby: u.is_a?(User)
来源：http://ati.jinyuanbaomall.cn

C#:   u is User
来源：http://xle.yuanzhike.top

[G14] 数据类 / record
来源：http://gwz.zhongyouzk.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://knh.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://jzl.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oaa.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://afa.cucudq.cn

Java: record User(String name, int age) {}
来源：http://mfi.shzxlz.cn

Go:   type User struct { Name string; Age int }
来源：http://uut.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cmt.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://pga.ppjwa.cn

[G15] 枚举
来源：http://frz.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cde.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xhx.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vyd.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://esx.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://uqz.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wsk.nwbrower.top

Ruby: Color = %i[red green].freeze
来源：http://ewu.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://veq.bbcook.cn

[G16] 对象转数组 / 字典
来源：http://juj.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kcx.cdnleiting.top

PHP:  get_object_vars($obj);
来源：http://lik.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://yoa.zdbjq.cn

TS:   Object.entries(obj)
来源：http://zmy.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ixb.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uwb.ybcxt.top

Ruby: obj.instance_variables
来源：http://gmc.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://pxx.52xcode.cn

================================================================================
来源：http://ynf.aibaodan.cn

H. 异常与错误处理
来源：http://jnp.shanyushiyangkeji.top

================================================================================
来源：http://dws.ivvv.top

[H01] try / catch 基础
来源：http://vfj.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qrl.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ulj.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ypp.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tkl.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://loh.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iip.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ezs.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ihl.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://teo.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iqv.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dng.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://adl.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://chn.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oqi.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://yeb.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xmu.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wba.hesvh.cn

[H03] 主动抛出异常
来源：http://spa.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://dlu.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nen.ppjwa.cn

JS:   throw new Error("错误信息");
来源：http://tqq.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://cxv.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://chy.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bbf.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xkn.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://mjl.havefunace.top

[H04] 自定义异常类型
来源：http://kqv.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://ajc.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://rdn.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://fxz.hnqzz.top

TS:   class MyError extends Error {}
来源：http://jwk.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://slo.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xba.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://sad.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://bsk.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://met.vehdjk.com

Py:   except ValueError as e:
来源：http://dsj.bbcook.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qug.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://dnu.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://reu.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://qti.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yzp.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://zag.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ikd.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://pua.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://hrb.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://jvc.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://gey.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://cso.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ogu.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cxj.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://skh.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://nfx.gzhubu.top

[H07] 断言
来源：http://wsq.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://erg.shzxlz.cn

PHP:  assert($x > 0);
来源：http://gen.wangdashe.top

JS:   console.assert(x > 0);
来源：http://azt.iojbl.cn

TS:   console.assert(x > 0);
来源：http://xpf.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://wvb.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qdt.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://izn.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://yqk.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://gbt.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://oqk.meibo888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kkl.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://drg.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wri.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wtu.pycfn.com

Go:   err.Error()
来源：http://ibi.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://hqn.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://qub.redwolf501.top

[H09] 带错误码的异常
来源：http://ujv.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sao.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ntz.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://coi.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bkv.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bcd.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nbp.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://eow.quarkkingdee.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qtg.fengsongda.top

[H10] 资源自动释放
来源：http://ugc.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://oox.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nrb.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bej.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://esn.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xph.bjfxy.top

Go:   defer f.Close()
来源：http://cip.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://avu.jinyuanbaomall.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qjc.haohaochexian.top

================================================================================
来源：http://cuf.jinghuilouyu.cn

I. 正则表达式
来源：http://pxa.gzhubu.top

================================================================================
来源：http://ofp.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://buq.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vii.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://odd.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://xmu.nwbrower.top

TS:   /\d+/.test(s)
来源：http://zso.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zjm.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ert.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://lbk.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ivq.ppjwa.cn

[I02] 提取所有匹配
来源：http://ipu.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://fmq.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uft.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wgw.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://ggc.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wlt.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://epd.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://qay.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bye.jianghu66.top

[I03] 提取捕获分组
来源：http://erc.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rlo.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://woy.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cte.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zdb.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ucp.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://njt.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rne.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://frx.yfazqb.com

[I04] 正则替换
来源：http://cxh.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://owc.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gnf.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://awc.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://xmy.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ztq.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ass.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fbh.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xdx.snrcjt.cn

[I05] 按正则拆分
来源：http://mnb.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hem.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lbw.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://dcr.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://kva.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://bsk.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ezg.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://mol.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ujl.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://inp.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dgs.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fqy.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yie.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://klz.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://inl.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fje.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fjl.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qkm.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://aqo.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ogw.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://chp.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mgq.daxiang520.top

TS:   /error/gim
来源：http://shf.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mcv.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jql.cashguo.top

Ruby: s.scan(/error/i)
来源：http://fxn.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hjz.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://lyl.daria6918.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xcq.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nfi.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sxg.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://get.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sxg.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nvi.yangfankeji.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mbg.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xpy.havefunace.top

================================================================================
来源：http://giu.ywan-chungtsiang.top

J. 日期与时间
来源：http://wpy.yfazqb.com

================================================================================
来源：http://eop.feifeiyinyue.top

[J01] 获取当前时间
来源：http://umo.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://txf.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://llu.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://zta.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://oln.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://mud.bjfxy.top

Go:   time.Now()
来源：http://ogb.yj20258.top

Ruby: Time.now
来源：http://jzj.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lcb.ctjpmb.com

[J02] 格式化输出
来源：http://zvl.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vgc.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://avh.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://puq.shzxlz.cn

TS:   d.toISOString()
来源：http://tlp.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gjq.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jem.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dip.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fnl.nwbrower.top

[J03] 字符串解析为日期
来源：http://mwc.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uif.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gmb.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://igt.bbcook.cn

TS:   new Date("2024-01-02")
来源：http://gae.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://olt.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://elg.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://eup.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hyn.guannengcc.top

[J04] 时间戳与日期互转
来源：http://okh.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yly.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fuv.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ywf.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fjv.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hpd.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ejw.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iew.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ewl.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://qhe.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://oyo.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nxz.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ake.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://axz.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://jbb.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ybb.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://mlk.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yuq.sxryk.cn

[J06] 计算两时间之差
来源：http://cyt.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://dns.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://zrm.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yal.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sdf.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://pwf.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://ckk.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://xgr.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://lsp.xuanzx.com

[J07] 比较两个日期
来源：http://isl.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://cya.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ios.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://mat.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ufb.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dxs.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://crc.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://pwy.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://sxs.zhongyouzk.top

[J08] 提取年月日与星期
来源：http://bwa.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obp.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sgl.yj20258.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xhg.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rjn.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ale.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://set.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lbc.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://umu.yj20258.top

[J09] 时区处理
来源：http://ivv.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://djn.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kgk.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cai.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fah.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ekh.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wac.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bqs.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aeo.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://ymh.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sdk.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ubi.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fvr.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xvp.jinghuilouyu.cn


<!-- 参考信息 -->