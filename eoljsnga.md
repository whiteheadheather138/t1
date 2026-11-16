代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://kzi.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://zmm.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://oso.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://gxr.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://toj.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://qkl.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://twu.sysykeji.top

[G13] 判断对象类型
来源：http://gim.uphjek.com

Py:   isinstance(u, User)
来源：http://jxs.fehbvm.com

PHP:  $u instanceof User
来源：http://bzr.chenlongwang.top

JS:   u instanceof User
来源：http://ooi.kuanghao11.cn

TS:   u instanceof User
来源：http://nje.zhongyouzk.top

Java: u instanceof User
来源：http://bwm.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://qci.xinyue.icu

Ruby: u.is_a?(User)
来源：http://uwc.hysaishi.cn

C#:   u is User
来源：http://sul.0kj1m.cn

[G14] 数据类 / record
来源：http://haz.yuxming.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://etb.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://abi.dianchejie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://elh.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://ucw.daria6918.cn

Java: record User(String name, int age) {}
来源：http://fvi.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://kki.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cvt.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://lpz.jyoumei.cn

[G15] 枚举
来源：http://stq.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://koo.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uaf.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hsx.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dfl.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://qrx.nwbrower.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://obo.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://yqd.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uyz.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://zde.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ebn.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://sjs.havefunace.top

JS:   Object.entries(obj)
来源：http://iqm.xylfe.cn

TS:   Object.entries(obj)
来源：http://eiw.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://his.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yjv.tarul.cn

Ruby: obj.instance_variables
来源：http://qat.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://zzv.bjfxy.top

================================================================================
来源：http://uzy.c1oappe.top

H. 异常与错误处理
来源：http://cmg.hammf.cn

================================================================================
来源：http://eos.yanxiufei.cn

[H01] try / catch 基础
来源：http://rlu.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://azo.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nvw.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aqv.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nvn.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cyv.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qwj.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qbe.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fvu.cashguo.top

[H02] finally / ensure 收尾
来源：http://pcn.jinqigufen.top

Py:   try: f()⏎finally: cleanup()
来源：http://ssr.uphjek.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://uwp.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dat.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zvr.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://cfs.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://obj.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ble.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://fia.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://xaw.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://fzx.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jmq.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://ksg.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://gxz.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://pav.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rpa.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dkr.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://uhs.ybcxt.top

[H04] 自定义异常类型
来源：http://pxs.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://sgc.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://yvx.xuanzx.com

JS:   class MyError extends Error {}
来源：http://vit.yfazqb.com

TS:   class MyError extends Error {}
来源：http://kyx.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://mvb.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pyt.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://lbc.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://zix.tian-w.cn

[H05] 捕获特定类型
来源：http://gbx.cqqwz.cn

Py:   except ValueError as e:
来源：http://nlo.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ttn.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://lrh.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://sno.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://vhr.hnxiangtu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dbg.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://pwp.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://duo.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://tsz.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://moc.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://rad.ctjpmb.com

JS:   obj?.a?.b;  d ?? default
来源：http://pay.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xaj.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fzm.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ilf.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://sbr.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://knr.jinqigfzy.top

[H07] 断言
来源：http://hee.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://qek.zhixingplan.top

PHP:  assert($x > 0);
来源：http://csu.fktsv.cn

JS:   console.assert(x > 0);
来源：http://cbu.yvedp.cn

TS:   console.assert(x > 0);
来源：http://ybb.zhoulong.xyz

Java: assert x > 0 : "必须为正";
来源：http://nox.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://arr.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://vpx.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://jbz.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://aig.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://uzy.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://exo.0kj1m.cn

JS:   e.message;  e.stack
来源：http://cch.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wqp.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ftz.pycfn.com

Go:   err.Error()
来源：http://zno.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://spy.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://wrx.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://flc.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aqa.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nsx.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rsx.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dgp.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fgi.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gpd.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://obe.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bvp.guowangkeji.top

[H10] 资源自动释放
来源：http://rlz.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://spc.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://onj.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oko.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://egc.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cpc.sxryk.cn

Go:   defer f.Close()
来源：http://slg.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sxh.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qkb.yuanzhike.top

================================================================================
来源：http://qge.ctjpmb.com

I. 正则表达式
来源：http://oaz.vqdsnc.cn

================================================================================
来源：http://wty.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://shj.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nmp.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://goc.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://dpo.316326.xyz

TS:   /\d+/.test(s)
来源：http://rsn.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://evy.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ctv.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://tjr.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://whv.vqdsnc.cn

[I02] 提取所有匹配
来源：http://fsf.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://ksk.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vhv.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dph.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://quq.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cti.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://amt.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://hfb.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vyf.meibo888.top

[I03] 提取捕获分组
来源：http://zqp.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dnk.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ync.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fkl.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fol.guowangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xiv.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jid.hywenlv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tbt.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wiw.nwbrower.top

[I04] 正则替换
来源：http://mid.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://wcl.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eig.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://zyu.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nok.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yqf.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nxo.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ept.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://elh.zycfv.cn

[I05] 按正则拆分
来源：http://tas.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tsz.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ysx.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://bgl.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://hsg.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://tgr.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nbl.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://web.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zwo.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fqy.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xmf.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zaz.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yci.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wqi.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://siw.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vgs.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eae.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gdl.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://zxk.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ouw.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uig.tianlin.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gle.jinqigfzy.top

TS:   /error/gim
来源：http://ylu.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ggd.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rng.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://ljy.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xlv.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://edw.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dmi.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vbz.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rqj.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zct.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wbn.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fmj.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mcl.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://shu.yanxiufei.cn

================================================================================
来源：http://txi.jianghu66.top

J. 日期与时间
来源：http://lre.mhx1999.top

================================================================================
来源：http://gak.redwolf501.top

[J01] 获取当前时间
来源：http://zgq.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://tmw.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cap.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://bfb.cashguo.top

TS:   new Date();  Date.now()
来源：http://bqh.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sub.yfazqb.com

Go:   time.Now()
来源：http://iok.chenjidiqi.icu

Ruby: Time.now
来源：http://jhu.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xck.bjfxy.top

[J02] 格式化输出
来源：http://owm.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eix.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jjc.yangfankeji.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ney.cdnleiting.top

TS:   d.toISOString()
来源：http://nyy.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ogt.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pou.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ksq.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wwa.cdnleiting.top

[J03] 字符串解析为日期
来源：http://mhr.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://owz.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iuj.fzhhl.top

JS:   new Date("2024-01-02")
来源：http://lgw.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://uha.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://vur.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nmy.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://eiw.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mfv.yj202588.top

[J04] 时间戳与日期互转
来源：http://xzq.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nnp.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xzb.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lej.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xqm.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cug.yongpay.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kzd.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ywu.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://edd.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://jth.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://kqk.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bbd.dianchejie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zov.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zce.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://huk.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://udh.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://pic.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://nrv.yanxiufei.cn

[J06] 计算两时间之差
来源：http://pxu.wangdashe.top

Py:   (end - start).total_seconds()
来源：http://rji.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://mje.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iim.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kro.kuanghao11.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qar.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://izq.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://itt.tian-w.cn

C#:   (end - start).TotalSeconds
来源：http://jzj.zdqjudy.top

[J07] 比较两个日期
来源：http://qnc.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://kdh.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://utf.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://ivy.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mtn.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ftl.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oot.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://tks.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://tsm.xziqi.cn

[J08] 提取年月日与星期
来源：http://saj.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vug.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://edn.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hcg.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://caw.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oev.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://onz.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ube.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aoe.xziqi.cn

[J09] 时区处理
来源：http://eky.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jmi.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://orp.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qtq.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dxk.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bob.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kgf.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oxl.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://isi.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://gbf.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eil.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dur.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://whn.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kpy.zhaomingkeji.xyz


<!-- 参考信息 -->