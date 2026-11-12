代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://bvi.hcnkem.com

JS:   toString() { return this.name; }
来源：http://lvb.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://acb.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://ees.xuanzx.com

Go:   func (u User) String() string { return u.Name }
来源：http://xij.gzhubu.top

Ruby: def to_s; @name; end
来源：http://pco.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://lpm.fehbvm.com

[G13] 判断对象类型
来源：http://txs.ybcxt.top

Py:   isinstance(u, User)
来源：http://zrb.tanke756.top

PHP:  $u instanceof User
来源：http://ndh.tanke756.top

JS:   u instanceof User
来源：http://bes.wangdashe.top

TS:   u instanceof User
来源：http://kth.epnwcf.com

Java: u instanceof User
来源：http://vcj.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xsj.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://ufp.aibaodan.cn

C#:   u is User
来源：http://zvt.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://fql.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://upd.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://onj.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fjy.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://xsy.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://qqq.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://win.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tou.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://ulf.aizwys.cn

[G15] 枚举
来源：http://dbn.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hkg.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://dqt.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ocj.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bjt.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://msw.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ren.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://jac.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://clx.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://soq.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rve.jqgfzy.top

PHP:  get_object_vars($obj);
来源：http://qwv.mhx1999.top

JS:   Object.entries(obj)
来源：http://ioh.cucudq.cn

TS:   Object.entries(obj)
来源：http://tig.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zwl.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://obe.havefunace.top

Ruby: obj.instance_variables
来源：http://hmx.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://ttk.shangyingyoupin.top

================================================================================
来源：http://esx.jyoumei.cn

H. 异常与错误处理
来源：http://eym.smart0.xyz

================================================================================
来源：http://ute.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://rbq.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tjp.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whr.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tyo.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ziq.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cng.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sor.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yvs.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bgo.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://iaq.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://unp.ydjk.org.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ynm.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qxb.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://evq.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://twi.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gsj.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ytl.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kbg.haohaochexian.top

[H03] 主动抛出异常
来源：http://gvk.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://jww.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mtd.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://sam.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://mqr.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqx.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bzd.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sjy.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lyd.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://lfh.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://bbn.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://wer.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://wit.zhengqikj.top

TS:   class MyError extends Error {}
来源：http://hbt.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://lgz.ybcxt.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ybh.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://fza.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://igb.meibo888.top

[H05] 捕获特定类型
来源：http://rrn.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://wys.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ezb.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://abh.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://brm.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://bzd.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bmh.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://shf.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ble.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://atc.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://kar.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://eux.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cbx.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qtv.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jnz.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hoc.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://lal.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://vlb.ybcxt.top

[H07] 断言
来源：http://gvj.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://myd.hammf.cn

PHP:  assert($x > 0);
来源：http://cpp.tanke756.top

JS:   console.assert(x > 0);
来源：http://ogy.bjfxy.top

TS:   console.assert(x > 0);
来源：http://wfp.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://qkz.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mzm.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://fir.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://kbi.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://jho.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://git.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ysi.c1oappe.top

JS:   e.message;  e.stack
来源：http://uhi.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xod.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kos.zdbjq.cn

Go:   err.Error()
来源：http://quo.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://dkc.kuanghao11.cn

C#:   e.Message;  e.StackTrace
来源：http://utc.ydzc1.top

[H09] 带错误码的异常
来源：http://vom.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dtf.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ylo.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dmn.hcnkem.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yjv.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bbj.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qoc.yfazqb.com

Ruby: raise MyError.new("fail", 500)
来源：http://bgy.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ttu.xylfe.cn

[H10] 资源自动释放
来源：http://cnj.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wun.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jte.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yhx.chenjidiqi.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://msf.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lbg.smart0.xyz

Go:   defer f.Close()
来源：http://oap.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ozq.ctjpmb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eld.sweek.top

================================================================================
来源：http://dvf.jinyuanbaomall.cn

I. 正则表达式
来源：http://myw.guannengcc.top

================================================================================
来源：http://xze.yongpay.top

[I01] 判断是否匹配
来源：http://zqd.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lgn.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://zyy.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://fxx.smart0.xyz

TS:   /\d+/.test(s)
来源：http://wkw.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mzo.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ild.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://vcu.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gql.zhaomingkeji.xyz

[I02] 提取所有匹配
来源：http://hir.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://akm.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://etb.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://olu.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://djp.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://phz.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ffs.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://jqq.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hap.quarkkingdee.top

[I03] 提取捕获分组
来源：http://yku.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hta.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sun.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ehb.vehdjk.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mad.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mzo.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rza.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://toi.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hhi.jinqigufen.top

[I04] 正则替换
来源：http://ulk.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hwe.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqc.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wpw.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://wih.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://exf.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jcr.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://cvw.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vqg.snrcjt.cn

[I05] 按正则拆分
来源：http://ucf.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://zqe.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cdf.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://chd.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://gbm.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://lvd.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://buq.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://gvp.daxiang520.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iln.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hts.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rlm.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pqa.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://npc.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lyv.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vfx.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mdt.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hhu.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wwv.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://jie.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eae.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kgt.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bty.jianghu66.top

TS:   /error/gim
来源：http://anq.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xin.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yfx.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://myk.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fhg.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://fli.hnqzz.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://crt.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qfl.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rak.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tuk.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://rkn.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://afo.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kzx.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://srn.ppjwa.cn

================================================================================
来源：http://gws.wangdashe.top

J. 日期与时间
来源：http://ldk.fehbvm.com

================================================================================
来源：http://sve.jinqigufen.top

[J01] 获取当前时间
来源：http://xqg.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fnm.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vvy.yj20258888.top

JS:   new Date();  Date.now()
来源：http://kvz.sysykeji.top

TS:   new Date();  Date.now()
来源：http://jph.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://puf.andypj.xyz

Go:   time.Now()
来源：http://lkn.tianlin.xyz

Ruby: Time.now
来源：http://uum.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lad.c1oappe.top

[J02] 格式化输出
来源：http://czo.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cxg.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ffc.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wca.ctjpmb.com

TS:   d.toISOString()
来源：http://wxo.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yqw.vqdsnc.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xzi.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gjc.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://txr.yuanzhike.top

[J03] 字符串解析为日期
来源：http://rwq.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bzr.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://edu.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://vwz.xuetiantiany.cn

TS:   new Date("2024-01-02")
来源：http://nme.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://uyo.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wph.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://mcs.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ivm.yueranfly.top

[J04] 时间戳与日期互转
来源：http://pnv.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gry.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kbj.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ljk.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://daw.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jtv.9152youxi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zsj.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fkq.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://obj.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://ixq.cashguo.top

Py:   now + timedelta(days=7)
来源：http://iiy.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gdn.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fck.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ctn.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://shl.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bfa.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://quw.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://phm.ppjwa.cn

[J06] 计算两时间之差
来源：http://rer.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://ahu.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://axz.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cli.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vju.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://anx.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://ryq.dianchejie.cn

Ruby: end - start                 # 返回秒数
来源：http://ysx.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://zok.daxiang520.top

[J07] 比较两个日期
来源：http://ocj.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://ysx.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wgt.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pwc.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://lmm.haohaochexian.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oiu.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lhs.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cry.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ofi.shuidangran.top

[J08] 提取年月日与星期
来源：http://rjx.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bxh.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bwz.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://koy.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yvj.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gmd.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cow.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tcb.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kdn.hammf.cn

[J09] 时区处理
来源：http://cxj.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ogg.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fjw.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://trs.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axf.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nrc.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tff.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://awe.tian-w.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dvu.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://kqg.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qsy.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://awj.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pwv.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rjm.jinghuilouyu.cn


<!-- 参考信息 -->