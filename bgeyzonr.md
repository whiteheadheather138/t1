代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://mon.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://lzj.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://frr.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://mul.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://rjf.smart0.xyz

Ruby: def to_s; @name; end
来源：http://iwh.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://fdp.wangdashe.top

[G13] 判断对象类型
来源：http://jfw.jiagoushi.top

Py:   isinstance(u, User)
来源：http://nxl.sxryk.cn

PHP:  $u instanceof User
来源：http://sfb.zdbjq.cn

JS:   u instanceof User
来源：http://hyw.shangyingyoupin.top

TS:   u instanceof User
来源：http://fsz.gaohongyu789.top

Java: u instanceof User
来源：http://zvb.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dev.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://cei.fehbvm.com

C#:   u is User
来源：http://kky.sufxvd.cn

[G14] 数据类 / record
来源：http://mcn.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://anl.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://uul.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://msb.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://vql.ivvv.top

Java: record User(String name, int age) {}
来源：http://etk.smart0.xyz

Go:   type User struct { Name string; Age int }
来源：http://ppz.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://woh.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://kvp.jinyuanbaomall.cn

[G15] 枚举
来源：http://hnk.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tqo.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://cxx.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rcz.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://udu.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://vxr.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://odd.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://lvt.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kqh.pycfn.com

[G16] 对象转数组 / 字典
来源：http://klo.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cah.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://phl.fzhhl.top

JS:   Object.entries(obj)
来源：http://cup.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://qnk.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bsw.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://tvj.xuetiantiany.cn

Ruby: obj.instance_variables
来源：http://wmm.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://fcu.hcnkem.com

================================================================================
来源：http://slt.chenjidiqi.icu

H. 异常与错误处理
来源：http://wyp.bjfxy.top

================================================================================
来源：http://nns.hfpthk.cn

[H01] try / catch 基础
来源：http://fhs.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tba.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ugp.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jms.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wbx.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dnr.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kuc.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xtx.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xem.cheryme.top

[H02] finally / ensure 收尾
来源：http://ssu.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://oro.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://twi.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://opy.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ipa.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://ncw.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pow.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zlc.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://cqr.ivvv.top

[H03] 主动抛出异常
来源：http://ker.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://ton.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kid.sweek.top

JS:   throw new Error("错误信息");
来源：http://uhk.xylfe.cn

TS:   throw new Error("错误信息");
来源：http://lua.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://htw.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hbk.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aql.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://egk.dashuyun.cn

[H04] 自定义异常类型
来源：http://jlj.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://tpp.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://xzy.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://hir.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://vvw.yuanzhike.top

Java: class MyException extends RuntimeException {}
来源：http://hjj.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tlf.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://our.fengsongda.top

C#:   class MyException : Exception {}
来源：http://adx.andypj.xyz

[H05] 捕获特定类型
来源：http://dui.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://qkz.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ziy.sjlbkw.cn

JS:   if (e instanceof TypeError) {}
来源：http://bxc.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://lbq.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://gla.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mdu.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://bfw.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://arv.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://ejc.sxryk.cn

Py:   value = d.get("k") or default
来源：http://fmi.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://sdq.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hmm.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://aeq.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gqs.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vlu.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://vbd.fzhhl.top

C#:   obj?.A?.B ?? default
来源：http://yjs.cucudq.cn

[H07] 断言
来源：http://ilg.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://rbe.xuanzx.com

PHP:  assert($x > 0);
来源：http://bsb.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://mml.shuidangran.top

TS:   console.assert(x > 0);
来源：http://udt.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://nev.zhoulong.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ijl.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://kwg.shanyushiyangtech.top

C#:   Debug.Assert(x > 0);
来源：http://zno.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://hzv.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://frz.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tng.yonumen.top

JS:   e.message;  e.stack
来源：http://gpe.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ijw.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rbv.ctjpmb.com

Go:   err.Error()
来源：http://gcl.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://fez.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://buy.ppjwa.cn

[H09] 带错误码的异常
来源：http://ksj.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ino.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vkp.jinqigufen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vme.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lnu.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rfd.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://let.redwolf501.top

Ruby: raise MyError.new("fail", 500)
来源：http://dja.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lag.zycfv.cn

[H10] 资源自动释放
来源：http://cyd.yanxiufei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nje.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fde.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aoa.dianchejie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rih.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mrt.cucudq.cn

Go:   defer f.Close()
来源：http://ukf.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://znl.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fis.dashuyun.cn

================================================================================
来源：http://ytg.shanyushiyangkeji.top

I. 正则表达式
来源：http://jvr.chenzaomai.com

================================================================================
来源：http://pbb.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://ovi.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://spm.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://agi.zycfv.cn

JS:   /\d+/.test(s)
来源：http://eej.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://wvy.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aow.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hft.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://gvi.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://voc.yfazqb.com

[I02] 提取所有匹配
来源：http://svb.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://khv.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lrg.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://apm.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://eiw.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aug.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zpa.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://abb.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dnu.xinyue.icu

[I03] 提取捕获分组
来源：http://qum.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xjj.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gwo.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ltr.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dtm.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qtg.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ujv.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lbz.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wbw.fktsv.cn

[I04] 正则替换
来源：http://fni.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lml.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ztu.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dof.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ibo.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://cxb.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pix.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fxx.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rxz.zdqjudy.top

[I05] 按正则拆分
来源：http://lsa.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://adi.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mlt.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://ile.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://yva.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://tjm.svipenyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dkn.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://wen.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://szs.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gld.xuanzx.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dig.dianchejie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nmk.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lzq.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oax.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bua.sjlbkw.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://czm.epnwcf.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wwm.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gzl.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://unf.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pse.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://puw.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uol.jqgufenzy.top

TS:   /error/gim
来源：http://yga.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qlk.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zbf.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://hzf.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vfc.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://gva.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fbj.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kkk.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cnj.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nzu.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rwr.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://emw.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gqx.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zdg.haohaochexian.top

================================================================================
来源：http://kyc.daria6918.cn

J. 日期与时间
来源：http://qop.fehbvm.com

================================================================================
来源：http://ibz.yueranfly.top

[J01] 获取当前时间
来源：http://adu.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fns.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hgn.yonumen.top

JS:   new Date();  Date.now()
来源：http://pca.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://nqj.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jol.yfazqb.com

Go:   time.Now()
来源：http://cwn.hongshengwenyu.top

Ruby: Time.now
来源：http://hhv.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ptg.cdnleiting.top

[J02] 格式化输出
来源：http://mlk.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ddw.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iwt.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://axg.wangdashe.top

TS:   d.toISOString()
来源：http://jpb.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cam.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oju.chenjidiqi.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sbp.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zgh.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://vnj.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hua.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qtx.pycfn.com

JS:   new Date("2024-01-02")
来源：http://mbi.xuanzx.com

TS:   new Date("2024-01-02")
来源：http://sjz.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://dxu.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ana.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://pvd.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ltv.iojbl.cn

[J04] 时间戳与日期互转
来源：http://rfg.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ull.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hty.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vhl.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cre.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://khb.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ers.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jvv.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jcm.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://jwb.cashguo.top

Py:   now + timedelta(days=7)
来源：http://lfc.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uot.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jzb.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ngq.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xqn.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://khl.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://scn.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://bft.zhijiandao.cn

[J06] 计算两时间之差
来源：http://uvy.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://wcc.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://yzx.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ezs.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uot.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gxa.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://wtk.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://obx.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://ygs.yj20258888.top

[J07] 比较两个日期
来源：http://ugx.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://pfs.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dfi.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://gbs.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://gmz.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wsl.0kj1m.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uif.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qiz.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://okq.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://rzi.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xib.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bim.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://anf.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bho.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://axd.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yxo.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fdd.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fag.havefunace.top

[J09] 时区处理
来源：http://gdq.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://djq.jqgfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mop.daria6918.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vse.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wvj.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sdk.chenlongwang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hvr.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nem.zhixingplan.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://icl.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://dnr.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hpg.ehwqpu.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kof.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nef.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fij.xziqi.cn


<!-- 参考信息 -->