代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://wzf.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://fsb.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://hym.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://tms.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://spc.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://lig.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://tut.wangshuangyany.cn

[G13] 判断对象类型
来源：http://lmg.gzhubu.top

Py:   isinstance(u, User)
来源：http://qjn.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://squ.gzhubu.top

JS:   u instanceof User
来源：http://kvx.xziqi.cn

TS:   u instanceof User
来源：http://psn.yj20258888.top

Java: u instanceof User
来源：http://rhy.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vsn.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://nqs.dianchejie.cn

C#:   u is User
来源：http://fli.hcnkem.com

[G14] 数据类 / record
来源：http://oar.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zyb.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://vlx.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rak.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://usz.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://ary.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://bfj.ydjk.org.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bxb.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://rct.hnxiangtu.top

[G15] 枚举
来源：http://mbm.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ygb.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://haf.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qvg.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tno.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://fzr.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kwt.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://dbl.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dom.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://gxd.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mhs.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://sna.zhixingplan.top

JS:   Object.entries(obj)
来源：http://rjc.yfazqb.com

TS:   Object.entries(obj)
来源：http://owf.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wfd.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ojf.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://dfs.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://jvh.dianchejie.cn

================================================================================
来源：http://ugf.sysykeji.top

H. 异常与错误处理
来源：http://bow.uphjek.com

================================================================================
来源：http://vjn.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://ykd.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uyw.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tsa.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zuu.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fcq.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cxr.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://niw.ehwqpu.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vri.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eum.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://dpm.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iza.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pfl.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://vrh.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sur.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yws.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://wtd.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://woe.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://orb.52xcode.cn

[H03] 主动抛出异常
来源：http://fsl.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://xgd.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dmq.cheryme.top

JS:   throw new Error("错误信息");
来源：http://hrl.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://gog.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ieo.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qko.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qjr.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kgb.chenlongwang.top

[H04] 自定义异常类型
来源：http://odp.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://krq.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://utl.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://llo.vqdsnc.cn

TS:   class MyError extends Error {}
来源：http://mtr.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://qrf.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yqw.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://ril.pycfn.com

C#:   class MyException : Exception {}
来源：http://csv.jiagoushi.top

[H05] 捕获特定类型
来源：http://iqm.cashguo.top

Py:   except ValueError as e:
来源：http://bxp.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eak.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://mqr.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://gcw.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://yjr.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ccq.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://zjm.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://acq.xuetiantiany.cn

[H06] 可选值 / 空值安全访问
来源：http://gdn.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://qiu.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://slq.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rzk.xingfuxueyuan.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://oyi.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kll.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mxm.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://kwl.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://xet.mhx1999.top

[H07] 断言
来源：http://rif.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://duy.cqqwz.cn

PHP:  assert($x > 0);
来源：http://jln.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://uic.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://lhn.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://vgw.cheryme.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://njp.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://uic.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://php.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://rmr.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://fph.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mpz.fehbvm.com

JS:   e.message;  e.stack
来源：http://xlm.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xnv.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://vyk.tarul.cn

Go:   err.Error()
来源：http://wik.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://gzn.shangyingyoupin.top

C#:   e.Message;  e.StackTrace
来源：http://vdp.guowangkeji.top

[H09] 带错误码的异常
来源：http://kok.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fwr.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vvn.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gjh.0kj1m.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://efm.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ddj.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://opk.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://jqp.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://eqz.gotoacloud.top

[H10] 资源自动释放
来源：http://bdv.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://afq.kuanghao11.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lvq.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hpf.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vzp.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xfc.xziqi.cn

Go:   defer f.Close()
来源：http://qsz.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fcp.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yxe.ydjk.org.cn

================================================================================
来源：http://lmo.fktsv.cn

I. 正则表达式
来源：http://jvz.tian-w.cn

================================================================================
来源：http://wqq.yanxiufei.cn

[I01] 判断是否匹配
来源：http://bdx.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://myo.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://ptd.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://xgd.hammf.cn

TS:   /\d+/.test(s)
来源：http://ocj.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fih.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fne.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://ikh.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dna.hnqzz.top

[I02] 提取所有匹配
来源：http://zdq.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://uvm.sufxvd.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zmz.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qll.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://djc.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bci.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ydu.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://vcw.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ymo.zhijiandao.cn

[I03] 提取捕获分组
来源：http://ekv.mhx1999.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fyv.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nkq.zdbjq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lxy.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ksi.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bwz.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lkl.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jfd.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rrk.shuidangran.top

[I04] 正则替换
来源：http://twc.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vsy.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpm.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://euc.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://kie.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://wch.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wwk.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vqz.tarul.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vau.nwbrower.top

[I05] 按正则拆分
来源：http://gmy.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://qpm.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bou.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://iod.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://yjr.hywenlv.cn

Java: s.split("\\s*,\\s*")
来源：http://mte.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hgg.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xat.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ojw.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zoj.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vdz.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://khm.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vyw.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wvq.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cqo.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://edr.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kcs.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://alj.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://jjy.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fbh.fehbvm.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rpm.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xwm.zhoulong.xyz

TS:   /error/gim
来源：http://lub.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uog.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://imw.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://sxw.ivvv.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xaf.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://cxr.yonumen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://knk.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hyd.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xlz.cheryme.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xfj.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cok.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vwl.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dey.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://voy.jiagoushi.top

================================================================================
来源：http://hbc.zhixingplan.top

J. 日期与时间
来源：http://gii.xuanzx.com

================================================================================
来源：http://mte.jqgufenzy.top

[J01] 获取当前时间
来源：http://wwg.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yno.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ntn.daxiang520.top

JS:   new Date();  Date.now()
来源：http://glf.uphjek.com

TS:   new Date();  Date.now()
来源：http://nyy.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dqa.yueranfly.top

Go:   time.Now()
来源：http://mmg.jiagoushi.top

Ruby: Time.now
来源：http://xwo.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lvs.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://ehc.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uvk.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fox.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://awx.smart0.xyz

TS:   d.toISOString()
来源：http://bbl.vehdjk.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iud.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fze.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qpm.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cui.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://qbg.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kkp.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jym.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://oon.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://zbi.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://czd.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://czu.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://mcx.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kzs.hcnkem.com

[J04] 时间戳与日期互转
来源：http://ezw.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bnt.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vad.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://npj.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dmf.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uuu.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kmj.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eil.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ejb.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://dpn.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://var.jiagoushi.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://uxb.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ens.zdbjq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fvn.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://rvt.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xxi.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://clp.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://opf.yj20258888.top

[J06] 计算两时间之差
来源：http://yva.pengpengdd.cyou

Py:   (end - start).total_seconds()
来源：http://hct.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://zvm.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ilw.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ufo.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://idx.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://ylh.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://tfy.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://xfh.zhongyouzk.top

[J07] 比较两个日期
来源：http://zii.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://hbu.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sbj.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://yql.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://urq.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qlc.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hii.quarkkingdee.top

Ruby: d1 < d2;  d1 == d2
来源：http://tsh.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://qny.fengsongda.top

[J08] 提取年月日与星期
来源：http://ifv.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://exc.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kkd.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ucw.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://usg.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kte.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ykk.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qar.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rud.birdmap.top

[J09] 时区处理
来源：http://isr.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dxz.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lza.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbm.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pln.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pxq.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wpn.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iun.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mwy.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://xjb.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jsm.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://llo.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zkg.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://irz.ehwqpu.com


<!-- 参考信息 -->