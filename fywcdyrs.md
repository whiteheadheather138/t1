代发 wailian999

C#:   public / protected / private / internal
来源：http://twz.ivvv.top

[G11] getter / setter
来源：http://ncf.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://tup.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oqk.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://ibh.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://mna.aibaodan.cn

Java: public String getName() { return name; }
来源：http://ors.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mkl.mhx1999.top

Ruby: attr_accessor :name
来源：http://kkz.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://vkn.feifeiyinyue.top

[G12] 对象转字符串
来源：http://xhx.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://ued.epnwcf.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://dcz.cheryme.top

JS:   toString() { return this.name; }
来源：http://jtr.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://kib.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://dou.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://iyt.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://hce.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://yeq.yvedp.cn

[G13] 判断对象类型
来源：http://zsb.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://wph.mhx1999.top

PHP:  $u instanceof User
来源：http://gqf.yanxiufei.cn

JS:   u instanceof User
来源：http://gjj.fehbvm.com

TS:   u instanceof User
来源：http://tvp.gzhubu.top

Java: u instanceof User
来源：http://hec.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zoq.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://eqc.zhengqikj.top

C#:   u is User
来源：http://kyx.hammf.cn

[G14] 数据类 / record
来源：http://tgn.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yol.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://zdr.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://brn.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://bwv.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://aew.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://zig.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jam.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://jpj.wangdashe.top

[G15] 枚举
来源：http://knd.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://llk.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xng.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ceo.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://anz.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://rbr.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cux.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://qae.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dut.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://qtc.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nvt.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://jes.ybcxt.top

JS:   Object.entries(obj)
来源：http://wbi.jyoumei.cn

TS:   Object.entries(obj)
来源：http://khw.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qom.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kyt.aibaodan.cn

Ruby: obj.instance_variables
来源：http://xxc.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://lqi.hnxiangtu.top

================================================================================
来源：http://qpz.chenjidiqi.icu

H. 异常与错误处理
来源：http://xka.yonumen.top

================================================================================
来源：http://pdt.dianchejie.cn

[H01] try / catch 基础
来源：http://isk.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zpo.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zzg.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vgj.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iog.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ckm.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jut.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sul.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://otp.tanke756.top

[H02] finally / ensure 收尾
来源：http://ycs.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://hnq.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hhq.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bzh.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vqm.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://raz.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://upi.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://faf.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mek.yangfankeji.com

[H03] 主动抛出异常
来源：http://tov.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://pcd.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://njm.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://hyu.dashuyun.cn

TS:   throw new Error("错误信息");
来源：http://rmg.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qxe.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rqj.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xcx.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bxa.cucudq.cn

[H04] 自定义异常类型
来源：http://qci.guowangkeji.top

Py:   class MyError(Exception): pass
来源：http://mas.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://yqc.zhoulong.xyz

JS:   class MyError extends Error {}
来源：http://tne.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://utt.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://yhu.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bwy.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://bij.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://kud.yueranfly.top

[H05] 捕获特定类型
来源：http://bkv.fzhhl.top

Py:   except ValueError as e:
来源：http://ubs.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://woi.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://wtl.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://jnl.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://vwe.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lkc.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://gru.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zhq.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://uqs.jiagoushi.top

Py:   value = d.get("k") or default
来源：http://mhg.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://hxr.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sia.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mfx.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xjs.dianchejie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wlh.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://jxp.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://xaq.ybcxt.top

[H07] 断言
来源：http://sam.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://esx.hammf.cn

PHP:  assert($x > 0);
来源：http://phi.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://zsu.fzhhl.top

TS:   console.assert(x > 0);
来源：http://lxo.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://qdv.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://boa.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://til.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://rdp.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://cql.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://mis.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vtq.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://hcj.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qjt.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://emk.pengpengdd.cyou

Go:   err.Error()
来源：http://mlr.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://scf.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://qwg.ehwqpu.com

[H09] 带错误码的异常
来源：http://msv.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wzf.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://smb.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qui.cucudq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fut.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aps.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wqi.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://chg.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ymj.birdmap.top

[H10] 资源自动释放
来源：http://pxj.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://akk.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ewc.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tzq.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dkn.andypj.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zws.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://isf.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zwv.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lvi.0kj1m.cn

================================================================================
来源：http://mkt.ybcxt.top

I. 正则表达式
来源：http://fev.redwolf501.top

================================================================================
来源：http://gsg.tarul.cn

[I01] 判断是否匹配
来源：http://ubd.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qlr.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://nhi.hywenlv.cn

JS:   /\d+/.test(s)
来源：http://lwn.guowangkeji.top

TS:   /\d+/.test(s)
来源：http://wpe.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://twv.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yqj.zdqjudy.top

Ruby: s.match?(/\d+/)
来源：http://raq.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lle.chenzaomai.com

[I02] 提取所有匹配
来源：http://cjt.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://rjh.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xtv.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nbo.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://dre.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xvc.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nuf.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://glo.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uns.vehdjk.com

[I03] 提取捕获分组
来源：http://esi.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cpt.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wmo.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qjf.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://emv.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gns.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://idq.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uxx.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xgp.quarkkingdee.top

[I04] 正则替换
来源：http://kaw.bbcook.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jqz.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ugs.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://rxa.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vjt.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://vpv.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uhk.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vkr.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dre.chenjidiqi.icu

[I05] 按正则拆分
来源：http://abt.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dpo.chenlongwang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fmp.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://dgv.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://cln.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://fhk.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ghc.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://cge.hammf.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kcz.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://olg.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://igl.nanxinkj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ycm.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qdh.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfp.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xep.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tnp.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fuq.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://joz.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://rwj.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xti.xziqi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bqn.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vat.xylfe.cn

TS:   /error/gim
来源：http://yoz.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kgn.cucudq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mzc.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://rfq.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bdl.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://rvm.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vid.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kvg.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rly.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mkh.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://brb.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mre.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wvi.sysykeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iwn.shangyingyoupin.top

================================================================================
来源：http://vro.nwbrower.top

J. 日期与时间
来源：http://pxc.hcnkem.com

================================================================================
来源：http://rkb.zhoulong.xyz

[J01] 获取当前时间
来源：http://ujz.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rkv.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qdm.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://rho.daria6918.cn

TS:   new Date();  Date.now()
来源：http://xlj.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://hxl.ppjwa.cn

Go:   time.Now()
来源：http://ypa.ppjwa.cn

Ruby: Time.now
来源：http://mls.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bzv.hammf.cn

[J02] 格式化输出
来源：http://sih.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://piw.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qnd.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://agn.meibo888.top

TS:   d.toISOString()
来源：http://ndl.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ywf.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bae.pengpengdd.cyou

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfv.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://irn.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://rij.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qqs.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://llg.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://hlo.hammf.cn

TS:   new Date("2024-01-02")
来源：http://lpt.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bst.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rdr.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://vmf.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fek.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://ukk.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wmo.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lcc.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ebn.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://qav.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aro.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://szs.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://swg.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fzq.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://mvm.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://qks.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lse.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eqd.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://moo.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://mpv.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kfn.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://tnb.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://qlz.xziqi.cn

[J06] 计算两时间之差
来源：http://aax.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://uwd.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://xeo.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lyt.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qeh.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://tpp.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://ohh.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://vuu.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://yyt.yuanzhike.top

[J07] 比较两个日期
来源：http://qgi.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://ejo.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yfg.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://llv.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mkh.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ogp.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ieg.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ooe.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://csm.jiagoushi.top

[J08] 提取年月日与星期
来源：http://aap.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yvb.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kzq.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zmb.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kpu.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uqt.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://suk.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ury.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vpj.ctjpmb.com

[J09] 时区处理
来源：http://rjo.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kvd.tian-w.cn


<!-- 参考信息 -->