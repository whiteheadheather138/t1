代发 wailian999

TS:   public / protected / private
来源：http://pbx.yj20258888.top

Java: public / protected / private / 默认包级
来源：http://ouy.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rfl.chenjidiqi.icu

Ruby: public / protected / private
来源：http://ylj.jinqigufen.top

C#:   public / protected / private / internal
来源：http://bja.zhixingplan.top

[G11] getter / setter
来源：http://xmj.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://dfi.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://trc.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://mmo.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://apv.jianghu66.top

Java: public String getName() { return name; }
来源：http://ioa.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xlc.zdqjudy.top

Ruby: attr_accessor :name
来源：http://mzv.zycfv.cn

C#:   public string Name { get; set; }
来源：http://cui.wangshuangyany.cn

[G12] 对象转字符串
来源：http://ptx.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://ajs.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://owy.fehbvm.com

JS:   toString() { return this.name; }
来源：http://yjq.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://ctp.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://cqk.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://heh.uphjek.com

Ruby: def to_s; @name; end
来源：http://vhb.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://lgq.sufxvd.cn

[G13] 判断对象类型
来源：http://lop.hywenlv.cn

Py:   isinstance(u, User)
来源：http://mbj.gotoacloud.top

PHP:  $u instanceof User
来源：http://ujr.jianghu66.top

JS:   u instanceof User
来源：http://rcc.hysaishi.cn

TS:   u instanceof User
来源：http://tbr.sweek.top

Java: u instanceof User
来源：http://thh.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fkc.fzhhl.top

Ruby: u.is_a?(User)
来源：http://vzw.jinghuilouyu.cn

C#:   u is User
来源：http://ntl.sjlbkw.cn

[G14] 数据类 / record
来源：http://zly.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vme.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://put.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://eof.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://xak.316326.xyz

Java: record User(String name, int age) {}
来源：http://ecr.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://uhr.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ipj.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://rdu.cheryme.top

[G15] 枚举
来源：http://jxo.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bgb.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ztx.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vae.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ffb.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://qjz.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hid.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://htc.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jsd.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://kqm.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eci.yj202588.top

PHP:  get_object_vars($obj);
来源：http://cfb.chenzaomai.com

JS:   Object.entries(obj)
来源：http://tdw.fehbvm.com

TS:   Object.entries(obj)
来源：http://lef.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qro.52xcode.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vvt.cashguo.top

Ruby: obj.instance_variables
来源：http://yih.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://zyx.hfpthk.cn

================================================================================
来源：http://ene.snrcjt.cn

H. 异常与错误处理
来源：http://pus.zhixingplan.top

================================================================================
来源：http://zim.cdnleiting.top

[H01] try / catch 基础
来源：http://jbz.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ocp.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ipt.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dyg.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://smz.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qki.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qbr.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bkl.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yfd.epnwcf.com

[H02] finally / ensure 收尾
来源：http://smg.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://vuu.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tus.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rjp.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bbm.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://neo.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mlj.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mcv.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://neo.hnxiangtu.top

[H03] 主动抛出异常
来源：http://dkm.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://mih.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bhx.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://bza.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://esq.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qcd.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gae.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ovq.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://ltc.cashguo.top

[H04] 自定义异常类型
来源：http://eab.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://wjh.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://cmg.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://yzj.yonumen.top

TS:   class MyError extends Error {}
来源：http://wsx.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://eua.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pxo.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://ycp.hywenlv.cn

C#:   class MyException : Exception {}
来源：http://zsz.smart0.xyz

[H05] 捕获特定类型
来源：http://dxd.tanke756.top

Py:   except ValueError as e:
来源：http://jyl.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lfa.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://sfv.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://jil.nwbrower.top

Java: catch (IOException | SQLException e) {}
来源：http://zmu.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://asl.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://rqc.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jun.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://ecb.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://njb.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://jhw.ivvv.top

JS:   obj?.a?.b;  d ?? default
来源：http://mux.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rho.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hmf.hcnkem.com

Go:   if v, ok := m["k"]; ok { }
来源：http://hoy.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://bcm.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://jkh.xylfe.cn

[H07] 断言
来源：http://rpr.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://nqa.guowangkeji.top

PHP:  assert($x > 0);
来源：http://icx.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://xjt.hesvh.cn

TS:   console.assert(x > 0);
来源：http://gpn.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://qrl.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ghv.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://yhg.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://jrz.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://azz.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://bcm.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mmn.nanxinkj.top

JS:   e.message;  e.stack
来源：http://ufi.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pqh.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://rms.nanxinkj.top

Go:   err.Error()
来源：http://huv.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://rrm.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://fai.epnwcf.com

[H09] 带错误码的异常
来源：http://yob.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xnv.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hkm.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mce.quarkkingdee.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hlo.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cpj.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://snk.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://csg.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kyj.jqgufenzy.top

[H10] 资源自动释放
来源：http://zih.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rvi.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aoa.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jhc.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fxq.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ktm.sufxvd.cn

Go:   defer f.Close()
来源：http://sby.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fnw.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oup.jinqigufen.top

================================================================================
来源：http://ufw.hammf.cn

I. 正则表达式
来源：http://tza.yuanzhike.top

================================================================================
来源：http://cgu.guannengcc.top

[I01] 判断是否匹配
来源：http://htz.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aur.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ssq.52xcode.cn

JS:   /\d+/.test(s)
来源：http://fhx.shanyushiyangkeji.top

TS:   /\d+/.test(s)
来源：http://icc.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ail.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ydp.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://dfu.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yjl.hcnkem.com

[I02] 提取所有匹配
来源：http://sem.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://uar.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gzx.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qno.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://gwg.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://myx.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gup.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://iju.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vsn.xylfe.cn

[I03] 提取捕获分组
来源：http://pmh.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cvq.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gmw.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tnz.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sbh.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aoe.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gqg.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rhq.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://njb.epnwcf.com

[I04] 正则替换
来源：http://jee.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tod.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aes.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://ncw.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://jfg.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ddp.zhaomingkeji.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://syt.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uli.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uzz.hesvh.cn

[I05] 按正则拆分
来源：http://zpt.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jza.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rsa.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://qzw.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://zpg.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://wvw.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://etd.yuanzhike.top

Ruby: s.split(/\s*,\s*/)
来源：http://qar.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xln.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://njl.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qyj.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bge.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mvi.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tui.wangdashe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sgy.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qhy.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dpt.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nbx.yongpay.top

[I07] 忽略大小写与多行模式
来源：http://wzy.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hhy.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://czb.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tbq.iojbl.cn

TS:   /error/gim
来源：http://swt.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ccc.yvedp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hsj.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://bbp.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bde.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://xlj.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lor.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zyv.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dzz.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://egk.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://giy.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fow.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xmc.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uhx.sjlbkw.cn

================================================================================
来源：http://sqe.yfazqb.com

J. 日期与时间
来源：http://nht.fktsv.cn

================================================================================
来源：http://qfp.ydzc1.top

[J01] 获取当前时间
来源：http://jsz.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ajn.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sob.bjfxy.top

JS:   new Date();  Date.now()
来源：http://vhi.aizwys.cn

TS:   new Date();  Date.now()
来源：http://xbn.yfazqb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qat.zhijiandao.cn

Go:   time.Now()
来源：http://llf.yj20258888.top

Ruby: Time.now
来源：http://xxk.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xis.zhiwuduotai.top

[J02] 格式化输出
来源：http://axb.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ytv.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uoc.yj202588.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qmc.zycfv.cn

TS:   d.toISOString()
来源：http://tro.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cbp.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lex.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dqo.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://thf.ppjwa.cn

[J03] 字符串解析为日期
来源：http://fnw.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ive.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vad.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://waa.ivvv.top

TS:   new Date("2024-01-02")
来源：http://rcn.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tcw.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bde.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://ryv.yj20258.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://soy.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://veg.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mex.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eyg.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uik.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wjl.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qkn.xylfe.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ldm.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nqx.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://unq.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://fig.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://zvs.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://php.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://don.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lqg.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://qje.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://beq.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://qjw.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://pjq.jqgufenzy.top

[J06] 计算两时间之差
来源：http://rvk.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://tpf.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://olg.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://onv.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rgn.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://vec.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://arp.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://ypz.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://asa.xziqi.cn

[J07] 比较两个日期
来源：http://fku.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://qvf.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lvb.52xcode.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tom.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ynm.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://msi.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tnm.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://ikp.uphjek.com

C#:   d1 < d2;  d1 == d2
来源：http://qmx.c1oappe.top

[J08] 提取年月日与星期
来源：http://mdg.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bjt.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pkt.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qlm.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nxl.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jyj.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uhr.hnqzz.top


<!-- 参考信息 -->