代发 wailian999

JS:   get name() { return this._name; }
来源：http://tve.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://fxh.fzhhl.top

Java: public String getName() { return name; }
来源：http://kql.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ncr.sweek.top

Ruby: attr_accessor :name
来源：http://wqu.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://pbw.fktsv.cn

[G12] 对象转字符串
来源：http://iwi.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://prs.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://bsm.vehdjk.com

JS:   toString() { return this.name; }
来源：http://zxl.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://uul.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://moe.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fhl.birdmap.top

Ruby: def to_s; @name; end
来源：http://ikl.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://gpk.kuanghao11.cn

[G13] 判断对象类型
来源：http://xgm.hysaishi.cn

Py:   isinstance(u, User)
来源：http://arz.nanxuanxn.top

PHP:  $u instanceof User
来源：http://vcd.zdqjudy.top

JS:   u instanceof User
来源：http://uiu.daxiang520.top

TS:   u instanceof User
来源：http://vov.ehwqpu.com

Java: u instanceof User
来源：http://put.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://mrl.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://etp.kuanghao11.cn

C#:   u is User
来源：http://gip.zycfv.cn

[G14] 数据类 / record
来源：http://tuk.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wol.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://wnc.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mff.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://gzc.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://oml.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://wwu.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pud.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://hbb.316326.xyz

[G15] 枚举
来源：http://oov.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xwf.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pjw.snrcjt.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tym.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xsr.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://djb.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://viw.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://vpj.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rwg.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://kik.yj20258.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://avx.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://ayj.hfpthk.cn

JS:   Object.entries(obj)
来源：http://jeb.gogol.net.cn

TS:   Object.entries(obj)
来源：http://toe.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ekl.havefunace.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eqv.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://oao.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://crm.bbcook.cn

================================================================================
来源：http://nsn.xuetiantiany.cn

H. 异常与错误处理
来源：http://brq.zdbjq.cn

================================================================================
来源：http://qtl.hnqzz.top

[H01] try / catch 基础
来源：http://iiu.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jpt.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qqp.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://juq.hnqzz.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kih.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qqp.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://obp.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qsz.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://snl.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://ixq.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nww.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://iae.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://leh.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tde.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yrn.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uft.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://imi.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://eek.cqqwz.cn

[H03] 主动抛出异常
来源：http://fyb.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://wmn.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vyo.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://yoa.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://oln.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cng.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mib.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pwa.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ssm.9152youxi.cn

[H04] 自定义异常类型
来源：http://hlo.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://teg.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://bvv.cheryme.top

JS:   class MyError extends Error {}
来源：http://rou.sxryk.cn

TS:   class MyError extends Error {}
来源：http://esa.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://fqg.0kj1m.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://udo.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://svy.52xcode.cn

C#:   class MyException : Exception {}
来源：http://kwq.fehbvm.com

[H05] 捕获特定类型
来源：http://xrt.hysaishi.cn

Py:   except ValueError as e:
来源：http://mrz.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bws.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://pvz.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://qdg.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://kwe.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://szp.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://bvr.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eow.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://anv.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://lct.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://cng.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://ehw.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://nti.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ccy.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xdn.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://rkf.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://jek.ydzc1.top

[H07] 断言
来源：http://kfx.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://pmr.hfpthk.cn

PHP:  assert($x > 0);
来源：http://qag.fehbvm.com

JS:   console.assert(x > 0);
来源：http://mud.redwolf501.top

TS:   console.assert(x > 0);
来源：http://fhb.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://hpi.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hrm.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mme.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://veq.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://mtg.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://vwf.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ipj.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://ful.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lbk.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://vlz.wangshuangyany.cn

Go:   err.Error()
来源：http://ozq.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://eyf.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://cya.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://qdu.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pak.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oqw.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cbg.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tom.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fiu.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tqi.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lkz.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ady.ppjwa.cn

[H10] 资源自动释放
来源：http://adr.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://amr.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lwx.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hov.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dyo.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bcn.aibaodan.cn

Go:   defer f.Close()
来源：http://url.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xut.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aqb.sufxvd.cn

================================================================================
来源：http://qdb.cheryme.top

I. 正则表达式
来源：http://dut.ywan-chungtsiang.top

================================================================================
来源：http://zlz.fehbvm.com

[I01] 判断是否匹配
来源：http://yny.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jwe.yangfankeji.com

PHP:  preg_match('/\d+/', $s);
来源：http://vvl.52xcode.cn

JS:   /\d+/.test(s)
来源：http://fgf.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://sjm.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zmh.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ars.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://qfn.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ffv.yj202588.top

[I02] 提取所有匹配
来源：http://rqa.daxiang520.top

Py:   re.findall(r"\d+", s)
来源：http://ovj.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nql.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://noi.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://jxi.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uyk.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zqx.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://wbk.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://roo.jlsjyb.cn

[I03] 提取捕获分组
来源：http://nij.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dpj.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://szv.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hgn.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://elg.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nsd.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ybm.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yzt.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ldy.jiagoushi.top

[I04] 正则替换
来源：http://dbn.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bdm.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ipf.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://gzx.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://pfc.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eza.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://vsx.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sht.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://swe.bbcook.cn

[I05] 按正则拆分
来源：http://pph.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eiz.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sxv.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://icp.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://vxm.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://rrp.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ohr.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vur.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rdv.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vud.hnxiangtu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://art.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://axo.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zhv.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lag.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lzj.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nsn.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://twc.yfazqb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mdj.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://bvr.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vcq.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lth.jinqigufen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ehr.cheryme.top

TS:   /error/gim
来源：http://wcr.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ehb.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dho.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://ncp.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://edq.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://tbk.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cft.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gzt.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mrj.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vbz.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ysk.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vwy.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eov.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pxd.zhaomingkeji.xyz

================================================================================
来源：http://udm.epnwcf.com

J. 日期与时间
来源：http://vhg.hnqzz.top

================================================================================
来源：http://nkz.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://jry.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vgq.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qeq.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://jgo.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://yql.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pxk.cdnleiting.top

Go:   time.Now()
来源：http://oui.hongshengwenyu.top

Ruby: Time.now
来源：http://veo.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dyv.yvedp.cn

[J02] 格式化输出
来源：http://wdz.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fnl.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lvc.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zpe.zhijiandao.cn

TS:   d.toISOString()
来源：http://qsx.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fgb.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://htp.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sok.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://piv.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://gde.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eug.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dga.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://wig.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://jsk.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://iiu.shangyingyoupin.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jpm.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://wxm.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hrv.hammf.cn

[J04] 时间戳与日期互转
来源：http://qho.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://skp.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://foz.shzxlz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://udr.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lji.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://epa.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nao.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://srx.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hkc.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://gqs.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://fjv.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://acp.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lfj.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ifu.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://rfn.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hvd.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://gmt.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://lgr.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://bhx.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://ghw.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://dyk.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ect.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xrs.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://qkw.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://tgg.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://meo.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://roe.tarul.cn

[J07] 比较两个日期
来源：http://xen.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://bwz.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ueh.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://mtm.yuanzhike.top

TS:   d1.getTime() < d2.getTime()
来源：http://yvn.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mig.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://efl.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hwf.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://ptj.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://sin.gaohongyu789.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sof.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hsv.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wuv.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://quk.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jwo.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qao.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nla.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wpi.uphjek.com

[J09] 时区处理
来源：http://hzo.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dyi.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zvj.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://obm.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gra.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yyi.nanxinkj.top


<!-- 参考信息 -->