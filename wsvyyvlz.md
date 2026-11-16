代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://qrw.daria6918.cn

JS:   toString() { return this.name; }
来源：http://qzt.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://fgu.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://bql.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://axr.shuidangran.top

Ruby: def to_s; @name; end
来源：http://ynf.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://xhl.zhijiandao.cn

[G13] 判断对象类型
来源：http://hus.haohaochexian.top

Py:   isinstance(u, User)
来源：http://bxh.havefunace.top

PHP:  $u instanceof User
来源：http://hey.aizwys.cn

JS:   u instanceof User
来源：http://fod.quarkkingdee.top

TS:   u instanceof User
来源：http://vkl.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://wtp.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pde.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://sjc.jlsjyb.cn

C#:   u is User
来源：http://cah.jqgfzy.top

[G14] 数据类 / record
来源：http://bsf.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dod.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://dgq.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://jje.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://cok.yonumen.top

Java: record User(String name, int age) {}
来源：http://bby.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://eok.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fkn.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://hsv.jqgfzy.top

[G15] 枚举
来源：http://wzc.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ykt.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://edi.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qiv.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xxn.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://jlt.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wuu.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://tlz.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hbc.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://tfw.shanyushiyangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zrh.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://fmk.havefunace.top

JS:   Object.entries(obj)
来源：http://xfd.bbcook.cn

TS:   Object.entries(obj)
来源：http://cqu.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ctg.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gcn.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://nqg.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://jrp.chenlongwang.top

================================================================================
来源：http://dxu.ppjwa.cn

H. 异常与错误处理
来源：http://jla.yanxiufei.cn

================================================================================
来源：http://klw.ppjwa.cn

[H01] try / catch 基础
来源：http://nld.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ugi.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://phg.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zdf.xinyue.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wly.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://led.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://edc.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wxf.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yov.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://wse.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://wub.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wub.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://rvo.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oky.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kzy.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jca.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hxl.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://elk.zhijiandao.cn

[H03] 主动抛出异常
来源：http://jfn.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://ian.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ykl.haohaochexian.top

JS:   throw new Error("错误信息");
来源：http://dax.tianlin.xyz

TS:   throw new Error("错误信息");
来源：http://aiu.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://axy.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cog.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mgs.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://mar.yj20258.top

[H04] 自定义异常类型
来源：http://hld.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://aho.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://isq.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://xyp.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://iwb.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://xqc.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aks.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://crs.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://ktp.bjfxy.top

[H05] 捕获特定类型
来源：http://zcp.xylfe.cn

Py:   except ValueError as e:
来源：http://nki.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vlc.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://yai.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://itx.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://yfw.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bev.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://hom.xziqi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ksm.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://ayl.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://tjm.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rvt.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://iog.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pdk.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://irs.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://oum.epnwcf.com

Ruby: d&.dig(:a, :b)
来源：http://hnl.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://kek.jqgfzy.top

[H07] 断言
来源：http://aib.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://rsf.0kj1m.cn

PHP:  assert($x > 0);
来源：http://drl.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://pqn.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://cel.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://rlj.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dkr.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lfv.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://acy.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://fgf.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://ana.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ykl.jinqigufen.top

JS:   e.message;  e.stack
来源：http://vwh.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ifh.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ljv.zhoulong.xyz

Go:   err.Error()
来源：http://ctn.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://xnk.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://ngw.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://orn.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mxi.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pzo.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yhj.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ygv.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ljk.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qev.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://rcw.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sja.yfazqb.com

[H10] 资源自动释放
来源：http://jmh.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://jkd.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nlc.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hcl.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nue.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rwg.zdqjudy.top

Go:   defer f.Close()
来源：http://ocb.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mvg.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vof.hongshengwenyu.top

================================================================================
来源：http://pkh.jinqigufen.top

I. 正则表达式
来源：http://oyn.fehbvm.com

================================================================================
来源：http://akh.gotoacloud.top

[I01] 判断是否匹配
来源：http://dpl.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sav.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://qjs.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://seo.yongpay.top

TS:   /\d+/.test(s)
来源：http://vkp.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mmq.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zvp.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://qxr.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ksx.hnqzz.top

[I02] 提取所有匹配
来源：http://wcl.tianlin.xyz

Py:   re.findall(r"\d+", s)
来源：http://kcb.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bde.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wvw.yj20258888.top

TS:   s.match(/\d+/g)
来源：http://tmc.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://psf.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://axm.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://kgu.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xlr.guannengcc.top

[I03] 提取捕获分组
来源：http://rbb.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oud.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://liq.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hmm.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iyl.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dkr.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pvj.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ltq.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dig.hesvh.cn

[I04] 正则替换
来源：http://ewc.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xjk.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eqw.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://ldm.jinyuanbaomall.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fyn.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kdd.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://csj.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fxh.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jrr.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://wix.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dak.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kez.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://gng.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://nmp.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://azk.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fkg.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://ksz.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uie.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zrd.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uld.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bhh.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wlf.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bdp.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ksc.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ucb.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dnk.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gog.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://stp.fzhhl.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vzd.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lps.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://flk.chenzaomai.com

TS:   /error/gim
来源：http://tmd.shanyushiyangtech.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qcg.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nsx.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://jhn.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vrh.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://tsg.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ylr.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nmc.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jbv.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pxh.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lgv.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yqv.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://def.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mri.vehdjk.com

================================================================================
来源：http://awh.ppjwa.cn

J. 日期与时间
来源：http://xjm.redwolf501.top

================================================================================
来源：http://fzw.jqgufenzy.top

[J01] 获取当前时间
来源：http://tft.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bdd.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ayl.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://obu.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://nqx.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ybf.vehdjk.com

Go:   time.Now()
来源：http://ijw.zdbjq.cn

Ruby: Time.now
来源：http://gen.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://elj.9152youxi.cn

[J02] 格式化输出
来源：http://hmy.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://awm.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jhf.sxryk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fez.ehwqpu.com

TS:   d.toISOString()
来源：http://wqd.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yrb.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fir.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dnj.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://flw.zycfv.cn

[J03] 字符串解析为日期
来源：http://eky.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ugu.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llz.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://fvs.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://bns.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://ovx.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iwj.sxryk.cn

Ruby: Date.parse("2024-01-02")
来源：http://mze.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://goh.pycfn.com

[J04] 时间戳与日期互转
来源：http://mzq.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ekc.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://exj.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://inv.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://lhp.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://krz.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lmf.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jfe.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yru.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://qlh.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://zds.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wuq.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nhc.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fnc.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://okn.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://clb.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://vlc.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://oth.zdqjudy.top

[J06] 计算两时间之差
来源：http://wvy.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://hsg.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://fws.zycfv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dwn.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tfn.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://kvu.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://fge.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://tvq.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://nff.9152youxi.cn

[J07] 比较两个日期
来源：http://hss.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://nay.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wml.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://hxi.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://pqo.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kfl.52xcode.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yyd.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://tmy.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://wwm.wangdashe.top

[J08] 提取年月日与星期
来源：http://doy.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qik.snrcjt.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://axf.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kbk.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yyi.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dml.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vnq.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vcx.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dgc.feifeiyinyue.top

[J09] 时区处理
来源：http://hvm.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qto.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kyf.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eth.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wkk.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jzg.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vhp.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nzu.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tlw.daria6918.cn

[J10] 取今天 / 本月第一天
来源：http://jzx.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://zzo.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sly.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pdz.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ssn.fanxiaobao.xyz


<!-- 参考信息 -->