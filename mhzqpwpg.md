代发 wailian999

JS:   get name() { return this._name; }
来源：http://wdu.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://smn.jyoumei.cn

Java: public String getName() { return name; }
来源：http://xto.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tyr.ppjwa.cn

Ruby: attr_accessor :name
来源：http://dbr.gzhubu.top

C#:   public string Name { get; set; }
来源：http://anl.yj20258.top

[G12] 对象转字符串
来源：http://zom.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://uig.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://oaz.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://sjt.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://nll.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://lla.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://ify.pengpengdd.cyou

Ruby: def to_s; @name; end
来源：http://pit.cheryme.top

C#:   public override string ToString() => Name;
来源：http://wve.jqgfzy.top

[G13] 判断对象类型
来源：http://oxz.xziqi.cn

Py:   isinstance(u, User)
来源：http://taq.ehwqpu.com

PHP:  $u instanceof User
来源：http://ldg.snrcjt.cn

JS:   u instanceof User
来源：http://ceu.zhiwuduotai.top

TS:   u instanceof User
来源：http://nfj.yuanzhike.top

Java: u instanceof User
来源：http://dar.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://stq.316326.xyz

Ruby: u.is_a?(User)
来源：http://vao.daxiang520.top

C#:   u is User
来源：http://unq.ctjpmb.com

[G14] 数据类 / record
来源：http://ons.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ixw.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://eeg.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://blo.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://lgo.redwolf501.top

Java: record User(String name, int age) {}
来源：http://nbd.xuetiantiany.cn

Go:   type User struct { Name string; Age int }
来源：http://hkf.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bni.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://wet.gogol.net.cn

[G15] 枚举
来源：http://ued.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iot.guannengcc.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dva.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uvh.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dcq.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://hbd.gotoacloud.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tpn.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://qty.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cwj.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://gtz.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xzp.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://pjg.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://ixn.hfpthk.cn

TS:   Object.entries(obj)
来源：http://hkj.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mrn.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://afy.hnqzz.top

Ruby: obj.instance_variables
来源：http://oph.bjfxy.top

C#:   // 用反射或 System.Text.Json
来源：http://nyf.gzhubu.top

================================================================================
来源：http://fqy.zhixingplan.top

H. 异常与错误处理
来源：http://iza.andypj.xyz

================================================================================
来源：http://gtz.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://lda.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zdo.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rjp.shangyingyoupin.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fmv.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ere.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wje.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rnz.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qej.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cyp.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://yib.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://cmo.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nwe.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vpr.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cax.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://yjj.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kqp.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://asx.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fam.hesvh.cn

[H03] 主动抛出异常
来源：http://yzb.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://zxu.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sdq.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://zhy.yj202588.top

TS:   throw new Error("错误信息");
来源：http://kwq.yj20258.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xgg.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ufq.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://plf.haohaochexian.top

C#:   throw new ArgumentException("错误信息");
来源：http://wci.zhongyouzk.top

[H04] 自定义异常类型
来源：http://jsm.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://ivh.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cgo.xziqi.cn

JS:   class MyError extends Error {}
来源：http://wqu.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://thi.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://bjj.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vnc.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://pld.fehbvm.com

C#:   class MyException : Exception {}
来源：http://fvb.bjfxy.top

[H05] 捕获特定类型
来源：http://ftu.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://mfg.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xko.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://zso.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://jxj.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://wzv.hesvh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vqh.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://clv.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wky.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://dph.redwolf501.top

Py:   value = d.get("k") or default
来源：http://buh.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://hcb.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gvk.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://eea.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eja.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://frv.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://qax.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://qql.tianlin.xyz

[H07] 断言
来源：http://dmv.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://qdc.zycfv.cn

PHP:  assert($x > 0);
来源：http://pne.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://mqg.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://ess.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://scj.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wbj.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nlf.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://uss.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://rqa.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://wto.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qkm.cucudq.cn

JS:   e.message;  e.stack
来源：http://odh.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hwk.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nlm.vqdsnc.cn

Go:   err.Error()
来源：http://bxa.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://zkf.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://tpp.sufxvd.cn

[H09] 带错误码的异常
来源：http://mgb.ydzc1.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ujp.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://mts.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://afv.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pmu.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ttj.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rhn.guannengcc.top

Ruby: raise MyError.new("fail", 500)
来源：http://pft.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xgb.cucudq.cn

[H10] 资源自动释放
来源：http://qmp.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kkx.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eps.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kgk.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pne.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qqw.feifeiyinyue.top

Go:   defer f.Close()
来源：http://jzu.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qqa.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mjp.vehdjk.com

================================================================================
来源：http://zgx.jiagoushi.top

I. 正则表达式
来源：http://xrx.wangshuangyany.cn

================================================================================
来源：http://ubg.jinqigufen.top

[I01] 判断是否匹配
来源：http://pxa.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rib.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://nvl.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://lde.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://wao.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://isf.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://clk.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://wns.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ghy.tian-w.cn

[I02] 提取所有匹配
来源：http://bhi.tanke756.top

Py:   re.findall(r"\d+", s)
来源：http://yql.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vdu.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dwx.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://tfe.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oak.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://adr.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://ehu.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wbq.vehdjk.com

[I03] 提取捕获分组
来源：http://yve.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://poz.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ute.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jll.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eyv.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bem.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rit.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wjc.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ifg.yuxming.cn

[I04] 正则替换
来源：http://zpd.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rxf.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qqc.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://mkv.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://upd.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fnn.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://dkg.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jqx.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oce.chenjidiqi.icu

[I05] 按正则拆分
来源：http://tlz.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fox.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ebw.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://pgb.guannengcc.top

TS:   s.split(/\s*,\s*/)
来源：http://vey.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://jre.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zpx.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://gxt.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fwl.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jvi.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tim.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qhf.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ayu.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ftl.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fmb.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aux.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qot.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jbu.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://knx.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hvc.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wji.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hue.hcnkem.com

TS:   /error/gim
来源：http://rzf.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kqq.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://une.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://vvb.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nxa.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://exe.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://acv.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kyl.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hck.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iff.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ydo.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pru.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fgu.zycfv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wqd.nwbrower.top

================================================================================
来源：http://xsy.ydjk.org.cn

J. 日期与时间
来源：http://ojt.pengpengdd.cyou

================================================================================
来源：http://mif.xylfe.cn

[J01] 获取当前时间
来源：http://jqy.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://mat.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rbi.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://nay.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://igd.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qvs.nanxinkj.top

Go:   time.Now()
来源：http://hqs.xuanzx.com

Ruby: Time.now
来源：http://xmc.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tiw.zycfv.cn

[J02] 格式化输出
来源：http://xbj.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txz.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://reg.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ymb.jqgfzy.top

TS:   d.toISOString()
来源：http://alz.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kcq.shanyushiyangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://clf.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oya.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://klv.birdmap.top

[J03] 字符串解析为日期
来源：http://mvc.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rpk.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xlt.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://psr.0kj1m.cn

TS:   new Date("2024-01-02")
来源：http://zet.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://zwi.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ftr.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://bfd.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dpq.redwolf501.top

[J04] 时间戳与日期互转
来源：http://bcr.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://crr.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eyy.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tuz.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eiw.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yed.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bnr.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bsy.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yvk.yj202588.top

[J05] 时间加减（加 7 天）
来源：http://juf.iojbl.cn

Py:   now + timedelta(days=7)
来源：http://wlt.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wkb.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtr.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahx.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://vnt.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nak.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://yer.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://dtw.wangdashe.top

[J06] 计算两时间之差
来源：http://yha.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://kvd.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://gbp.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://msc.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jgk.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ygd.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://uwn.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://bcj.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://vpe.feifeiyinyue.top

[J07] 比较两个日期
来源：http://kki.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://rqa.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://arz.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nmb.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://eqt.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qtr.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hwb.fanxiaobao.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://zcz.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://ojj.sufxvd.cn

[J08] 提取年月日与星期
来源：http://tbw.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fmk.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vxd.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tjw.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wxu.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kgn.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dds.hysaishi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kmo.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nqj.gotoacloud.top

[J09] 时区处理
来源：http://hcd.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sjc.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zcy.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vtz.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sxv.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dbu.gzhubu.top


<!-- 参考信息 -->