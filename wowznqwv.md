代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rmc.cheryme.top

[Q75] 日期格式化
来源：http://xip.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pta.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rce.zhengqikj.top

[Q76] 按天统计
来源：http://nij.zhengqikj.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jdb.smart0.xyz

[Q77] 时间加减
来源：http://qfe.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://asu.jqgfzy.top

[Q78] 当前时间
来源：http://hkv.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ett.nanxinkj.top

[Q79] 字符串拼接
来源：http://asw.xuetiantiany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ebo.yuxming.cn

[Q80] 字符串截取
来源：http://wrs.yvedp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gid.gaohongyu789.top

[Q81] 字符串替换
来源：http://jch.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tfd.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://iwg.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kez.jlsjyb.cn

[Q83] 大小写转换
来源：http://vgq.aibaodan.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ujh.havefunace.top

[Q84] 去除首尾空格
来源：http://xlc.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://oda.dashuyun.cn

[Q85] 数值取整
来源：http://hud.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pvo.uphjek.com

[Q86] 读取 JSON 字段
来源：http://nvk.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dza.sxryk.cn

[Q87] JSON 字段做条件
来源：http://gig.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nvp.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://wks.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qjt.sweek.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dcy.haohaochexian.top

[Q89] 判断表是否存在
来源：http://npv.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://myb.tarul.cn

[Q90] 生成序号列
来源：http://jwg.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://leu.xuetiantiany.cn

================================================================================
来源：http://hih.cheryme.top

R. Bash 专题
来源：http://oeu.tian-w.cn

================================================================================
来源：http://nju.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://qcr.xylfe.cn

#!/usr/bin/env bash
来源：http://tef.ydzc1.top

set -euo pipefail
来源：http://cyn.zdbjq.cn

[R02] 变量赋值与使用
来源：http://wda.gotoacloud.top

name="Tom"; echo "$name"
来源：http://pmc.yj20258888.top

[R03] 只读变量
来源：http://grc.316326.xyz

readonly PI=3.14
来源：http://dgi.xuanzx.com

[R04] 位置参数
来源：http://ktn.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xzc.pycfn.com

[R05] 参数默认值
来源：http://utr.hysaishi.cn

name="${1:-default}"
来源：http://pxm.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://vtr.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jun.zhixingplan.top

[R07] if 判断文件
来源：http://twb.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pwk.yangfankeji.com

[R08] 数值比较
来源：http://aok.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tcz.nanxuanxn.top

[R09] 字符串比较
来源：http://djc.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fpb.sjlbkw.cn

[R10] 正则匹配
来源：http://pzo.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xiy.yj20258888.top

[R11] case 多分支
来源：http://uya.hnqzz.top

case "$1" in
来源：http://mmi.hnxiangtu.top

start) echo "启动" ;;
来源：http://rbh.zhixingplan.top

stop)  echo "停止" ;;
来源：http://oby.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://eem.fehbvm.com

esac
来源：http://yaq.birdmap.top

[R12] for 遍历文件
来源：http://jzn.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://bzc.andypj.xyz

[R13] for 计数循环
来源：http://zst.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://lrz.yj202588.top

[R14] C 风格 for
来源：http://dbk.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://khb.hnqzz.top

[R15] while 逐行读文件
来源：http://qni.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fpd.fzhhl.top

[R16] until 等待条件
来源：http://nga.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://scg.shzxlz.cn

[R17] 数组定义与取值
来源：http://qto.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://pmz.kuanghao11.cn

[R18] 遍历数组
来源：http://inl.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://doo.gaohongyu789.top

[R19] 数组长度
来源：http://dkk.bjfxy.top

echo "${#arr[@]}"
来源：http://jmn.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://hgk.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lsp.9152youxi.cn

[R21] 字符串长度
来源：http://yxt.havefunace.top

echo "${#s}"
来源：http://yrf.sufxvd.cn

[R22] 截取子串
来源：http://hey.52xcode.cn

echo "${s:0:5}"
来源：http://jnf.fktsv.cn

[R23] 字符串替换
来源：http://mbg.shuidangran.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wfc.zdqjudy.top

[R24] 大小写转换
来源：http://jna.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://fud.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://etr.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fes.vehdjk.com

[R26] 命令替换
来源：http://idt.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://fdn.zhengqikj.top

[R27] 算术展开
来源：http://mqb.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://bbe.redwolf501.top

[R28] 浮点运算
来源：http://qag.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://ufd.yfazqb.com

[R29] 定义函数
来源：http://uvz.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ryt.epnwcf.com

[R30] 函数返回状态码
来源：http://wlf.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ink.vqdsnc.cn

[R31] 局部变量
来源：http://ckl.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://mdq.zdqjudy.top

[R32] 参数个数校验
来源：http://zca.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hjc.hammf.cn

[R33] 捕获错误并提示行号
来源：http://ekg.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gkq.jinqigfzy.top

[R34] 退出时清理
来源：http://eqc.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://ael.quarkkingdee.top

[R35] 后台执行并等待
来源：http://qcy.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://liz.wangdashe.top

[R36] 并发执行多个任务
来源：http://kzd.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kft.yfazqb.com

[R37] 把输出赋给变量
来源：http://upr.sjlbkw.cn

files=$(ls -1)
来源：http://mgl.tanke756.top

[R38] 管道串联
来源：http://wtm.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://zem.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://uwu.nanxinkj.top

cmd > out.log 2>&1
来源：http://mzl.0kj1m.cn

[R40] 追加写日志
来源：http://ali.pycfn.com

echo "log" >> out.log
来源：http://ttv.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://cet.nwbrower.top

cmd >/dev/null 2>&1
来源：http://ooc.havefunace.top

[R42] 输入重定向
来源：http://sxx.feifeiyinyue.top

wc -l < a.txt
来源：http://iyu.bjfxy.top

[R43] 按名字查找文件
来源：http://hqk.wangdashe.top

find . -name "*.log" -type f
来源：http://ghb.52xcode.cn

[R44] 按修改时间查找
来源：http://mop.zdbjq.cn

find . -mtime -7 -type f
来源：http://qzt.yj20258.top

[R45] 批量删除
来源：http://zry.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://vaq.gotoacloud.top

[R46] 递归替换文件内容
来源：http://iex.316326.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cfb.wangdashe.top

[R47] sed 单行替换
来源：http://wzv.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://jha.bjfxy.top

[R48] awk 取指定列
来源：http://yre.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://pnz.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://qqz.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jmr.tianlin.xyz

[R50] awk 求和
来源：http://aiv.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://wmv.zhijiandao.cn

[R51] 排序去重取前几
来源：http://nyz.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://get.zhongyouzk.top

[R52] 统计行数
来源：http://skd.tanke756.top

wc -l a.txt
来源：http://kmo.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://dgs.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ybj.zhoulong.xyz

[R54] 比较两个文件
来源：http://wfe.hysaishi.cn

diff a.txt b.txt
来源：http://blv.fengsongda.top

[R55] 压缩与解压
来源：http://sqe.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://onx.mhx1999.top

[R56] 远程拷贝
来源：http://zqe.hnxiangtu.top

scp file user@host:/path/
来源：http://oce.ehwqpu.com

[R57] 远程执行命令
来源：http://rsb.pycfn.com

ssh user@host 'uptime'
来源：http://uvl.yvedp.cn

[R58] 下载文件
来源：http://xbx.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qth.quarkkingdee.top

[R59] 发 POST JSON
来源：http://zsw.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://miw.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://ljm.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://biv.tianlin.xyz

[R61] 磁盘占用
来源：http://xjw.gotoacloud.top

df -h;  du -sh *
来源：http://vvw.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://esh.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://xch.wangshuangyany.cn

[R63] 内存与进程
来源：http://xhz.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://wtr.guowangkeji.top

[R64] 结束进程
来源：http://hfi.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://zey.sufxvd.cn

[R65] 查看端口占用
来源：http://qjk.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ltf.zhiwuduotai.top

[R66] 定时任务
来源：http://zgo.chenlongwang.top

crontab -e;  crontab -l
来源：http://div.pycfn.com

[R67] 生成随机十六进制串
来源：http://wsa.52xcode.cn

openssl rand -hex 16
来源：http://vtb.cheryme.top

[R68] 计算文件校验值
来源：http://zyp.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mmr.smart0.xyz

[R69] 生成随机密码
来源：http://shw.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://eqg.tian-w.cn

[R70] 时间戳与互转
来源：http://pvh.yj202588.top

date +%s;  date -d @1700000000
来源：http://vvr.yanxiufei.cn

[R71] 日期格式化
来源：http://mti.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ngt.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://thl.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yzb.meibo888.top

[R73] 分割大日志
来源：http://nso.andypj.xyz

split -l 1000 big.log part_
来源：http://zhb.0kj1m.cn

[R74] 批量重命名
来源：http://eim.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jss.shangyingyoupin.top

[R75] 导出环境变量
来源：http://zie.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://bcw.tianlin.xyz

[R76] 使用临时文件
来源：http://jlk.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpt.vqdsnc.cn

[R77] 读取用户输入
来源：http://yhn.jinqigufen.top

read -rp "请输入: " ans
来源：http://ovv.hcnkem.com

[R78] 交互式菜单
来源：http://fqs.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://jhz.ydzc1.top

[R79] 解析命令行选项
来源：http://otp.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xab.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://hcc.zhaomingkeji.xyz

time ./run.sh
来源：http://drk.yuxming.cn

================================================================================
来源：http://qsw.zdbjq.cn

S. C / C++ 专题
来源：http://awv.tianlin.xyz

================================================================================
来源：http://nge.guowangkeji.top

[S01] C：Hello World
来源：http://kxi.hcnkem.com

#include <stdio.h>
来源：http://gfh.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lsc.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://cee.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://gny.nanxuanxn.top

[S03] C：读入整数
来源：http://nwz.cashguo.top

int x; scanf("%d", &x);
来源：http://fdn.ctjpmb.com

[S04] C：字符串复制
来源：http://jav.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://yyw.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://zor.guannengcc.top

strlen(s)
来源：http://dwh.yj20258888.top

[S06] C：字符串比较
来源：http://ohw.pycfn.com

strcmp(a, b) == 0
来源：http://arf.cucudq.cn

[S07] C：数组遍历求和
来源：http://ydf.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jdf.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://kwq.jinyuanbaomall.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://caj.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://vej.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://awo.pycfn.com

[S10] C：指针与解引用
来源：http://iig.iojbl.cn

int *p = &a;  *p = 5;
来源：http://yox.ppjwa.cn

[S11] C：逐行读文件
来源：http://fjt.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://xrl.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://flg.yanxiufei.cn

fclose(f);
来源：http://usl.vqdsnc.cn

[S12] C：写文件
来源：http://eki.yongpay.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tsy.jiagoushi.top

[S13] C：宏定义
来源：http://uov.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ojx.birdmap.top

[S14] C：枚举
来源：http://ikh.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://vth.hnxiangtu.top

[S15] C：类型转换
来源：http://ltv.316326.xyz

(double) a / b
来源：http://yqm.aibaodan.cn

[S16] C：位操作置位
来源：http://spw.yfazqb.com

x |= (1 << 3);
来源：http://trx.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://xzz.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wmk.sufxvd.cn

[S18] C：命令行参数
来源：http://eql.ydjk.org.cn

int main(int argc, char **argv)
来源：http://ldr.zdqjudy.top

[S19] C：快速排序
来源：http://nyq.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://eal.daxiang520.top

[S20] C：二分查找
来源：http://zrh.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nny.yj202588.top

[S21] C：字符类别判断
来源：http://qwb.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ymi.xylfe.cn

[S22] C：字符串转数字
来源：http://hea.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://hns.yongpay.top

[S23] C：随机数
来源：http://lsp.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://faz.tianlin.xyz

[S24] C：获取本地时间
来源：http://deu.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xlq.hcnkem.com

[S25] C：内存拷贝
来源：http://ptb.bbcook.cn

memcpy(dst, src, n);
来源：http://heq.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://adn.pycfn.com

memset(a, 0, sizeof a);
来源：http://dgo.9152youxi.cn

[S27] C：定义常量
来源：http://lei.yueranfly.top

const double PI = 3.14159;
来源：http://wma.nanxinkj.top

[S28] C：静态变量
来源：http://bmc.sweek.top

static int counter = 0;
来源：http://ynx.yangfankeji.com

[S29] C：变参函数
来源：http://wzo.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bju.cucudq.cn

[S30] C：头文件保护
来源：http://ops.quarkkingdee.top

#ifndef X_H
来源：http://iza.nanxuanxn.top

#define X_H
来源：http://ihq.yangfankeji.com

#endif
来源：http://vhf.yfazqb.com

[S31] C++：Hello World
来源：http://nik.guowangkeji.top

#include <iostream>
来源：http://moa.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://lqo.xziqi.cn

[S32] C++：字符串
来源：http://hgo.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://zoj.yueranfly.top

[S33] C++：vector 增删
来源：http://nnj.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cju.316326.xyz

[S34] C++：遍历 vector
来源：http://twk.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://hkt.gaohongyu789.top

[S35] C++：map
来源：http://anh.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pxb.yj20258888.top

[S36] C++：unordered_map
来源：http://tbh.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://psj.haohaochexian.top

[S37] C++：set
来源：http://clj.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vly.wangshuangyany.cn

[S38] C++：排序
来源：http://ets.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://yua.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://urx.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wag.hywenlv.cn

[S40] C++：查找元素
来源：http://lfw.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://usd.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://sfd.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oiv.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://ewf.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://ykw.jiagoushi.top

[S43] C++：智能指针
来源：http://mdh.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://vhy.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://tfj.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://uwe.sweek.top


<!-- 参考信息 -->