代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://uvw.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://hhl.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://rqo.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://rkr.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://xqj.bjfxy.top

Ruby: def to_s; @name; end
来源：http://cik.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://xlh.ydzc1.top

[G13] 判断对象类型
来源：http://ybz.snrcjt.cn

Py:   isinstance(u, User)
来源：http://iwp.jianghu66.top

PHP:  $u instanceof User
来源：http://vdl.gogol.net.cn

JS:   u instanceof User
来源：http://uen.yuxming.cn

TS:   u instanceof User
来源：http://ihu.smart0.xyz

Java: u instanceof User
来源：http://loz.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tcm.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://kop.ybcxt.top

C#:   u is User
来源：http://hwc.zdqjudy.top

[G14] 数据类 / record
来源：http://hlq.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zkb.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://dst.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://ywm.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://zyk.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://jgg.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://wvk.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://icv.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://haq.jlsjyb.cn

[G15] 枚举
来源：http://gep.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://byo.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zem.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://brm.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qpe.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://lwu.tianlin.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hff.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://dag.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ybm.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://rzc.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kfs.yongpay.top

PHP:  get_object_vars($obj);
来源：http://uhr.shzxlz.cn

JS:   Object.entries(obj)
来源：http://owc.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://wfg.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ccs.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gpu.daria6918.cn

Ruby: obj.instance_variables
来源：http://neu.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://jba.bjfxy.top

================================================================================
来源：http://zbz.pengpengdd.cyou

H. 异常与错误处理
来源：http://cey.jianghu66.top

================================================================================
来源：http://eco.bjfxy.top

[H01] try / catch 基础
来源：http://sxk.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fyh.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gkk.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ikv.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ugt.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fip.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vna.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zno.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kuq.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://rei.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xjs.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fja.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hpr.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rnf.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://imc.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://osh.andypj.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://wsz.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://rve.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://lmg.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://nsk.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dfm.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://svq.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://rbo.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xro.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ngv.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fku.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://knu.mhx1999.top

[H04] 自定义异常类型
来源：http://jbk.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://pkv.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://gwp.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://leg.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://ezm.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://atw.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gtk.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://jpv.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://qzw.sufxvd.cn

[H05] 捕获特定类型
来源：http://fkp.smart0.xyz

Py:   except ValueError as e:
来源：http://yyx.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://drm.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://nsb.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://lez.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://uab.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ijs.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://eko.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://epu.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://wrn.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://hgr.0kj1m.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jrd.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://auw.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://yuo.daxiang520.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kkf.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://els.yuanzhike.top

Ruby: d&.dig(:a, :b)
来源：http://opc.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://zaw.gogol.net.cn

[H07] 断言
来源：http://yyy.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://jrb.fehbvm.com

PHP:  assert($x > 0);
来源：http://ckg.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://gen.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://cxh.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://qnc.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qyo.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://ren.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://oof.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://coj.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://ytg.sjlbkw.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rlm.cucudq.cn

JS:   e.message;  e.stack
来源：http://hdx.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rjg.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://xuo.jinyuanbaomall.cn

Go:   err.Error()
来源：http://hrz.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://sjw.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://uge.smart0.xyz

[H09] 带错误码的异常
来源：http://img.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zrj.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vww.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kjg.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ktt.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sxd.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qya.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://uqp.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wpj.aibaodan.cn

[H10] 资源自动释放
来源：http://wsr.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hpx.yj202588.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ebo.ywan-chungtsiang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pbi.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fhr.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mrh.chenjidiqi.icu

Go:   defer f.Close()
来源：http://hng.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xoc.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iar.jyoumei.cn

================================================================================
来源：http://mqu.iojbl.cn

I. 正则表达式
来源：http://ikq.jyoumei.cn

================================================================================
来源：http://pau.tarul.cn

[I01] 判断是否匹配
来源：http://mle.pengpengdd.cyou

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qtr.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jno.52xcode.cn

JS:   /\d+/.test(s)
来源：http://kvb.mhx1999.top

TS:   /\d+/.test(s)
来源：http://qwy.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xid.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://try.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://ele.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vyy.gogol.net.cn

[I02] 提取所有匹配
来源：http://yty.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://kfx.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hlv.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tuv.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://qkd.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hht.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://grx.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://pgx.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ghz.cqqwz.cn

[I03] 提取捕获分组
来源：http://ldq.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://csx.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vgf.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://clt.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aef.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kku.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://foy.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dzh.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nok.tarul.cn

[I04] 正则替换
来源：http://tou.jiagoushi.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bqo.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nyt.gaohongyu789.top

JS:   s.replace(/\d+/g, "#")
来源：http://ntg.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://axx.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sre.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bmj.c1oappe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ygc.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tvj.hongshengwenyu.top

[I05] 按正则拆分
来源：http://xsj.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://old.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wlc.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://fab.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://aed.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://xdz.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yld.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://hne.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qwz.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://okk.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lhd.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iep.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dce.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://opr.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gem.hammf.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wgb.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xig.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gzv.sweek.top

[I07] 忽略大小写与多行模式
来源：http://nhn.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fjx.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://djp.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://awo.hesvh.cn

TS:   /error/gim
来源：http://hhk.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aks.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tfj.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://xcx.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://btn.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://hni.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ipm.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vjh.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zlc.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wcl.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lnf.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ilc.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://whm.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fmi.xuetiantiany.cn

================================================================================
来源：http://wum.uphjek.com

J. 日期与时间
来源：http://qns.316326.xyz

================================================================================
来源：http://gvw.nanxinkj.top

[J01] 获取当前时间
来源：http://ani.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wrm.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wuw.shangyingyoupin.top

JS:   new Date();  Date.now()
来源：http://fcn.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://tjz.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kju.bbcook.cn

Go:   time.Now()
来源：http://zko.bbcook.cn

Ruby: Time.now
来源：http://ifm.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nfa.hywenlv.cn

[J02] 格式化输出
来源：http://yau.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dvq.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yrc.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yip.ppjwa.cn

TS:   d.toISOString()
来源：http://xkm.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ocf.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nch.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ntf.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://plg.dianchejie.cn

[J03] 字符串解析为日期
来源：http://csq.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://erw.redwolf501.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zdo.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://cdl.pycfn.com

TS:   new Date("2024-01-02")
来源：http://ndj.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://bii.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gsd.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://eww.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://osq.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://pqr.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tvp.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lfs.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sqy.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qpu.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bcg.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mrs.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zqt.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hvr.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://aoy.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://tkf.guannengcc.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gnt.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oee.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rnq.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://hcl.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gtm.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://hyj.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://dym.cdnleiting.top

[J06] 计算两时间之差
来源：http://rcr.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://sgi.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://fig.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hvi.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ghm.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://aaq.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://opq.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://hen.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://vak.vehdjk.com

[J07] 比较两个日期
来源：http://ede.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://bzd.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ztv.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pnc.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://ukb.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pbi.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://car.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://aca.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://tht.sweek.top

[J08] 提取年月日与星期
来源：http://twc.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xnm.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nbo.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nob.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kex.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dps.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jsx.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oiu.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wyl.aibaodan.cn

[J09] 时区处理
来源：http://fvf.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oth.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fvd.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywc.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://arg.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jeu.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mey.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qzz.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ixn.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://jwx.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dsb.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bhj.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://edu.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jks.ydzc1.top


<!-- 参考信息 -->