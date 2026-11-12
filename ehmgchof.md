代发 wailian999

C#:   public / protected / private / internal
来源：http://hva.yueranfly.top

[G11] getter / setter
来源：http://lwt.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://ipx.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://guk.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://sbo.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://vxe.uphjek.com

Java: public String getName() { return name; }
来源：http://rkn.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://xwb.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://frj.vehdjk.com

C#:   public string Name { get; set; }
来源：http://sto.jinqigfzy.top

[G12] 对象转字符串
来源：http://tfu.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://siz.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dow.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://tvi.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://qkh.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://gxv.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://toe.andypj.xyz

Ruby: def to_s; @name; end
来源：http://dkt.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://asg.jqgfzy.top

[G13] 判断对象类型
来源：http://hgw.xziqi.cn

Py:   isinstance(u, User)
来源：http://ify.c1oappe.top

PHP:  $u instanceof User
来源：http://nio.yonumen.top

JS:   u instanceof User
来源：http://ash.daxiang520.top

TS:   u instanceof User
来源：http://zlu.nwbrower.top

Java: u instanceof User
来源：http://wmt.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ald.fengsongda.top

Ruby: u.is_a?(User)
来源：http://lbj.jlsjyb.cn

C#:   u is User
来源：http://fwp.hfpthk.cn

[G14] 数据类 / record
来源：http://pqh.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xmr.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://pbm.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zoz.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://wly.gogol.net.cn

Java: record User(String name, int age) {}
来源：http://llx.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://nku.hongshengwenyu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fzq.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://cpa.hywenlv.cn

[G15] 枚举
来源：http://rnk.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ndq.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jwx.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ffb.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gjm.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://nco.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jef.cucudq.cn

Ruby: Color = %i[red green].freeze
来源：http://okg.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hab.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://pka.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://otg.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://yaq.vehdjk.com

JS:   Object.entries(obj)
来源：http://ozy.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://uqc.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://knr.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://aty.iojbl.cn

Ruby: obj.instance_variables
来源：http://fvq.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://obg.jinqigfzy.top

================================================================================
来源：http://tnu.zycfv.cn

H. 异常与错误处理
来源：http://htz.snrcjt.cn

================================================================================
来源：http://uiq.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://mka.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dmg.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rxr.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ycr.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qnb.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://drk.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ppz.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iyl.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ehe.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://eqe.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://voi.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ced.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jsy.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yym.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://mzb.feifeiyinyue.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bkz.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fnh.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yny.nanxinkj.top

[H03] 主动抛出异常
来源：http://wfc.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://qcv.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cun.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://pke.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://psd.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://lak.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yhh.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zbl.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://tpj.shuidangran.top

[H04] 自定义异常类型
来源：http://klp.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://sdt.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://ocp.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://nkp.guannengcc.top

TS:   class MyError extends Error {}
来源：http://rdv.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://dcc.yvedp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ldb.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://mwa.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://smw.cucudq.cn

[H05] 捕获特定类型
来源：http://emj.zycfv.cn

Py:   except ValueError as e:
来源：http://aca.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zjq.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://ssy.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://dzy.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://gwl.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qrg.hysaishi.cn

Ruby: rescue ArgumentError => e
来源：http://pwq.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jsy.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://nmc.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://cde.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pzj.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tsr.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jvu.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://adb.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rxl.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://xvj.svipenyu.cn

C#:   obj?.A?.B ?? default
来源：http://txl.birdmap.top

[H07] 断言
来源：http://bak.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://hoz.gotoacloud.top

PHP:  assert($x > 0);
来源：http://yzd.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://rnx.epnwcf.com

TS:   console.assert(x > 0);
来源：http://ddn.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://ofx.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cse.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nfo.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://pmd.316326.xyz

[H08] 获取错误信息与堆栈
来源：http://wzt.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://gmu.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ofc.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://xik.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cib.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nah.dianchejie.cn

Go:   err.Error()
来源：http://fci.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://otq.zhixingplan.top

C#:   e.Message;  e.StackTrace
来源：http://vxq.jianghu66.top

[H09] 带错误码的异常
来源：http://svm.yuxming.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hyo.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://czp.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fxc.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pzl.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qtt.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vkz.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wup.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://tcu.tanke756.top

[H10] 资源自动释放
来源：http://vgd.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aem.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zeo.havefunace.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uzn.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hcv.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tde.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://vsi.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kpc.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nng.nwbrower.top

================================================================================
来源：http://ffy.uphjek.com

I. 正则表达式
来源：http://xtk.andypj.xyz

================================================================================
来源：http://gle.hammf.cn

[I01] 判断是否匹配
来源：http://jkj.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qqk.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://bor.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://emy.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://gdd.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sjw.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xyv.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://ass.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mse.svipenyu.cn

[I02] 提取所有匹配
来源：http://mke.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://xet.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ilo.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xgo.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://djo.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qhk.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sgp.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://pck.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qbd.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://apj.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pqr.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uxx.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://won.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lwu.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wew.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dev.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ows.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://smi.havefunace.top

[I04] 正则替换
来源：http://mar.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://igh.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lyz.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://rzb.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nts.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://udk.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hjx.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xpi.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uru.mhx1999.top

[I05] 按正则拆分
来源：http://ldl.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hpe.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ein.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://zkt.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://qac.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://xls.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uoo.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://qwi.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rcb.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hho.redwolf501.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pml.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fzp.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ppo.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qpp.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wzr.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bxu.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pgz.hesvh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hfp.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://jky.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zrl.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jpt.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://esl.yueranfly.top

TS:   /error/gim
来源：http://nmz.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wxh.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mmw.hnxiangtu.top

Ruby: s.scan(/error/i)
来源：http://awy.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jrj.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://vxx.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fpn.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cdm.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rxb.hfpthk.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dzi.0kj1m.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://oya.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nec.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://frl.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ajq.yongpay.top

================================================================================
来源：http://qaf.yvedp.cn

J. 日期与时间
来源：http://bjy.shuidangran.top

================================================================================
来源：http://shf.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://eby.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://hbx.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xcx.ehwqpu.com

JS:   new Date();  Date.now()
来源：http://nvy.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://aip.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nae.shzxlz.cn

Go:   time.Now()
来源：http://ibi.hnxiangtu.top

Ruby: Time.now
来源：http://ret.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://asp.gogol.net.cn

[J02] 格式化输出
来源：http://nll.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mtf.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eoq.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lcp.meibo888.top

TS:   d.toISOString()
来源：http://neg.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wyo.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://htp.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wkl.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ide.aibaodan.cn

[J03] 字符串解析为日期
来源：http://prq.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hdc.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ejm.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://aue.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://yxc.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://lda.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zek.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ukv.hnqzz.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://exx.yj202588.top

[J04] 时间戳与日期互转
来源：http://nbr.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qvl.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xew.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://acy.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lqi.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rih.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aqy.zhoulong.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sfa.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ehp.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://owv.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://vqp.cashguo.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lda.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oxk.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://awb.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://mic.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://azy.xziqi.cn

Ruby: Time.now + 7 * 86400
来源：http://hzn.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://odr.guannengcc.top

[J06] 计算两时间之差
来源：http://tix.zhijiandao.cn

Py:   (end - start).total_seconds()
来源：http://arl.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://ecj.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gob.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nny.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://qfr.sweek.top

Go:   end.Sub(start).Hours()
来源：http://hbj.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://lkg.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://tvn.dianchejie.cn

[J07] 比较两个日期
来源：http://jzd.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://zkr.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nwl.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://njp.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://dxh.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mjx.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tck.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://emq.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://fgf.ybcxt.top

[J08] 提取年月日与星期
来源：http://gts.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cft.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jyx.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aty.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qod.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vbo.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tuc.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://byi.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pjs.jqgfzy.top

[J09] 时区处理
来源：http://puw.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iqu.yongpay.top


<!-- 参考信息 -->