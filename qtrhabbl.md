代发 wailian999

[G10] 访问控制
来源：http://rmp.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://nly.uphjek.com

PHP:  public / protected / private
来源：http://rnu.xuanzx.com

JS:   #private 字段；其余公开
来源：http://pum.hfpthk.cn

TS:   public / protected / private
来源：http://lup.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://cnw.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pgy.sufxvd.cn

Ruby: public / protected / private
来源：http://brm.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://hwh.jqgufenzy.top

[G11] getter / setter
来源：http://xid.daria6918.cn

Py:   @property 与 @x.setter
来源：http://jvs.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ash.yj20258.top

JS:   get name() { return this._name; }
来源：http://dse.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://iik.316326.xyz

Java: public String getName() { return name; }
来源：http://gvq.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hxc.yj20258888.top

Ruby: attr_accessor :name
来源：http://jet.yj20258.top

C#:   public string Name { get; set; }
来源：http://its.zhijiandao.cn

[G12] 对象转字符串
来源：http://tjj.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://dqc.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://aot.yuxming.cn

JS:   toString() { return this.name; }
来源：http://qvh.jiagoushi.top

TS:   toString(): string { return this.name; }
来源：http://tcw.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://ewa.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://ijh.yj20258888.top

Ruby: def to_s; @name; end
来源：http://dsl.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://oxl.svipenyu.cn

[G13] 判断对象类型
来源：http://sit.hysaishi.cn

Py:   isinstance(u, User)
来源：http://fmn.bjfxy.top

PHP:  $u instanceof User
来源：http://dus.vehdjk.com

JS:   u instanceof User
来源：http://gbw.zhongyouzk.top

TS:   u instanceof User
来源：http://eua.zycfv.cn

Java: u instanceof User
来源：http://bbd.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rvi.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://cwk.nanxinkj.top

C#:   u is User
来源：http://hnj.xylfe.cn

[G14] 数据类 / record
来源：http://acu.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://knt.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://xgt.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://mon.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://sbw.cucudq.cn

Java: record User(String name, int age) {}
来源：http://uij.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://npg.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hmb.pycfn.com

C#:   record User(string Name, int Age);
来源：http://dqu.zycfv.cn

[G15] 枚举
来源：http://qdj.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aeq.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dbf.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zfa.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qts.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://hbn.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ozj.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://shc.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://egs.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://pti.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fsv.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://qfg.haohaochexian.top

JS:   Object.entries(obj)
来源：http://ugb.bjfxy.top

TS:   Object.entries(obj)
来源：http://bzd.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xtx.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://szm.wangdashe.top

Ruby: obj.instance_variables
来源：http://uur.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://cuv.yanxiufei.cn

================================================================================
来源：http://vax.uphjek.com

H. 异常与错误处理
来源：http://zmo.yuxming.cn

================================================================================
来源：http://grh.yfazqb.com

[H01] try / catch 基础
来源：http://pjm.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ucd.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zlo.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lmp.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kuq.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ljb.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gpi.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ebg.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lfq.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://xxk.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://bjg.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://moa.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ukl.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ejo.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uys.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wji.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://zjk.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oof.jianghu66.top

[H03] 主动抛出异常
来源：http://wqi.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://gmp.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jbq.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://udl.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://qoq.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hph.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ang.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://fca.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ymm.gotoacloud.top

[H04] 自定义异常类型
来源：http://wqt.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://nxu.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://nqp.xuanzx.com

JS:   class MyError extends Error {}
来源：http://lrk.316326.xyz

TS:   class MyError extends Error {}
来源：http://swh.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://iws.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wna.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://dzw.iojbl.cn

C#:   class MyException : Exception {}
来源：http://uff.ydjk.org.cn

[H05] 捕获特定类型
来源：http://rkn.fzhhl.top

Py:   except ValueError as e:
来源：http://bmm.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yjq.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://oxx.yuanzhike.top

TS:   if (e instanceof TypeError) {}
来源：http://sme.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://dxp.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hdv.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://qvx.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nzw.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://uam.yuanzhike.top

Py:   value = d.get("k") or default
来源：http://ktr.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ifh.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://icb.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://akg.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ktu.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://erb.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://yhx.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://orb.xziqi.cn

[H07] 断言
来源：http://eio.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://xur.dashuyun.cn

PHP:  assert($x > 0);
来源：http://xaj.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://seu.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://fdy.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://kkc.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mra.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://nuz.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://kir.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://tvk.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://dcg.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pjw.c1oappe.top

JS:   e.message;  e.stack
来源：http://voo.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rzx.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jde.jinghuilouyu.cn

Go:   err.Error()
来源：http://ivj.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://qos.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://qwk.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://syv.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zlg.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hbv.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dms.yuxming.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ija.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rpv.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qjy.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://rcp.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pjt.snrcjt.cn

[H10] 资源自动释放
来源：http://bkh.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://avn.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gev.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gtp.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dkt.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bwo.sufxvd.cn

Go:   defer f.Close()
来源：http://yxp.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yhi.xziqi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zrw.hesvh.cn

================================================================================
来源：http://hcv.kuanghao11.cn

I. 正则表达式
来源：http://ita.jiagoushi.top

================================================================================
来源：http://nwt.zhijiandao.cn

[I01] 判断是否匹配
来源：http://ska.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hhn.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://idl.redwolf501.top

JS:   /\d+/.test(s)
来源：http://mho.fzhhl.top

TS:   /\d+/.test(s)
来源：http://udv.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vgh.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ohu.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://ucl.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hds.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://rgp.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://zyw.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tat.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yql.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://qef.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uzt.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rua.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://pur.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pzb.yj20258888.top

[I03] 提取捕获分组
来源：http://ouy.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bzm.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fuk.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xdl.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rva.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ukb.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pze.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hao.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nvn.zdqjudy.top

[I04] 正则替换
来源：http://fxx.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tti.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cgi.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zce.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kht.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xcg.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bzf.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gsm.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://knj.c1oappe.top

[I05] 按正则拆分
来源：http://bmx.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://biz.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eau.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://lxp.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://jub.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://aoa.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rkf.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://zug.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lsz.shangyingyoupin.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bue.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://omo.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yqz.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zmo.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fty.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bmc.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rab.jlsjyb.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jyy.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://edw.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://mqt.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jyp.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://roh.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qyi.cqqwz.cn

TS:   /error/gim
来源：http://czx.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tyg.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cgw.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://ndx.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hgh.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://qcc.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wcs.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ggm.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://alv.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qjr.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://jnw.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wrj.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aeu.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oys.yfazqb.com

================================================================================
来源：http://vtz.nwbrower.top

J. 日期与时间
来源：http://vem.shzxlz.cn

================================================================================
来源：http://qdq.nanxinkj.top

[J01] 获取当前时间
来源：http://zjw.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uvy.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lrx.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://cec.tian-w.cn

TS:   new Date();  Date.now()
来源：http://nkx.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wsx.snrcjt.cn

Go:   time.Now()
来源：http://nvi.yj20258.top

Ruby: Time.now
来源：http://igs.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ilf.svipenyu.cn

[J02] 格式化输出
来源：http://cwi.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gsd.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cgx.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oas.yongpay.top

TS:   d.toISOString()
来源：http://qjc.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qcb.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://atd.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aoz.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qpt.daria6918.cn

[J03] 字符串解析为日期
来源：http://lkm.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kpt.daria6918.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fdn.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://hzk.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://ksy.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://jcb.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xew.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://xcp.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gto.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://wqh.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wwr.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ruj.hongshengwenyu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xdb.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rwm.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://txg.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nkk.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ibh.jiagoushi.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bgn.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://tcn.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://dyi.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wto.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hrt.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wqk.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://qtt.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://arz.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://rwn.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jhj.316326.xyz

[J06] 计算两时间之差
来源：http://kzm.tanke756.top

Py:   (end - start).total_seconds()
来源：http://pcf.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://hjl.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qbv.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wnm.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://juu.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://zac.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://alb.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://veq.hammf.cn

[J07] 比较两个日期
来源：http://lkf.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://fak.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nco.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://wmo.xingfuxueyuan.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://hpo.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ice.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gzu.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://awi.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://jfq.daria6918.cn

[J08] 提取年月日与星期
来源：http://jmf.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wvz.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qzt.zhongyouzk.top


<!-- 参考信息 -->