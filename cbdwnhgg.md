代发 wailian999

[Q76] 按天统计
来源：http://mos.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://itn.shzxlz.cn

[Q77] 时间加减
来源：http://igx.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cpk.zhijiandao.cn

[Q78] 当前时间
来源：http://njs.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://inl.jianghu66.top

[Q79] 字符串拼接
来源：http://bfw.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ias.hongshengwenyu.top

[Q80] 字符串截取
来源：http://vtw.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xps.kuanghao11.cn

[Q81] 字符串替换
来源：http://dgh.zhoulong.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ywh.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://kdu.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://brk.wangshuangyany.cn

[Q83] 大小写转换
来源：http://ogv.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kag.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://zdc.haohaochexian.top

SELECT TRIM(name) FROM users;
来源：http://zoo.jqgfzy.top

[Q85] 数值取整
来源：http://uin.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://luq.hongshengwenyu.top

[Q86] 读取 JSON 字段
来源：http://hwh.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fga.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://thd.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cpt.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://utd.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qak.zdqjudy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uhr.nanxinkj.top

[Q89] 判断表是否存在
来源：http://qzp.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xxu.yj20258888.top

[Q90] 生成序号列
来源：http://iaa.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rgm.jyoumei.cn

================================================================================
来源：http://hvn.gaohongyu789.top

R. Bash 专题
来源：http://rrl.cucudq.cn

================================================================================
来源：http://dzj.zycfv.cn

[R01] shebang 与严格模式
来源：http://kje.yfazqb.com

#!/usr/bin/env bash
来源：http://cgv.hysaishi.cn

set -euo pipefail
来源：http://xth.c1oappe.top

[R02] 变量赋值与使用
来源：http://jxt.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://iih.yueranfly.top

[R03] 只读变量
来源：http://bgf.aizwys.cn

readonly PI=3.14
来源：http://plq.yj20258888.top

[R04] 位置参数
来源：http://sch.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lqc.sxryk.cn

[R05] 参数默认值
来源：http://czf.nwbrower.top

name="${1:-default}"
来源：http://fpm.fktsv.cn

[R06] 判断命令是否存在
来源：http://htw.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nrr.feifeiyinyue.top

[R07] if 判断文件
来源：http://ael.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yuu.smart0.xyz

[R08] 数值比较
来源：http://jiv.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://jsz.nanxuanxn.top

[R09] 字符串比较
来源：http://yac.guannengcc.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fmo.daria6918.cn

[R10] 正则匹配
来源：http://iln.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vin.cheryme.top

[R11] case 多分支
来源：http://pra.zdbjq.cn

case "$1" in
来源：http://nmw.quarkkingdee.top

start) echo "启动" ;;
来源：http://vrl.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://xkq.ybcxt.top

*)     echo "未知命令" ;;
来源：http://sks.shanyushiyangkeji.top

esac
来源：http://ilp.hfpthk.cn

[R12] for 遍历文件
来源：http://zge.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://tfo.guowangkeji.top

[R13] for 计数循环
来源：http://kiz.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://jst.feifeiyinyue.top

[R14] C 风格 for
来源：http://lfx.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vob.jqgfzy.top

[R15] while 逐行读文件
来源：http://zzk.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lxm.pycfn.com

[R16] until 等待条件
来源：http://zhs.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yvg.ydjk.org.cn

[R17] 数组定义与取值
来源：http://ksn.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ukl.jqgfzy.top

[R18] 遍历数组
来源：http://zee.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mjt.9152youxi.cn

[R19] 数组长度
来源：http://btz.tarul.cn

echo "${#arr[@]}"
来源：http://yad.chenzaomai.com

[R20] 关联数组（字典）
来源：http://zhk.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vaz.yj202588.top

[R21] 字符串长度
来源：http://xwl.ivvv.top

echo "${#s}"
来源：http://hgd.chenzaomai.com

[R22] 截取子串
来源：http://qep.tianlin.xyz

echo "${s:0:5}"
来源：http://uzb.hnxiangtu.top

[R23] 字符串替换
来源：http://zov.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gyc.feifeiyinyue.top

[R24] 大小写转换
来源：http://khe.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://ynb.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://ozc.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://cae.shanyushiyangtech.top

[R26] 命令替换
来源：http://aex.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://rml.bbcook.cn

[R27] 算术展开
来源：http://vzp.tarul.cn

echo $((1 + 2 * 3))
来源：http://jal.sysykeji.top

[R28] 浮点运算
来源：http://xmr.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://sgs.yvedp.cn

[R29] 定义函数
来源：http://fuf.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bay.cheryme.top

[R30] 函数返回状态码
来源：http://dqk.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://itb.havefunace.top

[R31] 局部变量
来源：http://yyi.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://eul.feifeiyinyue.top

[R32] 参数个数校验
来源：http://xxz.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://okh.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://gee.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qas.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://etu.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://cti.jyoumei.cn

[R35] 后台执行并等待
来源：http://hmk.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://mzw.zdbjq.cn

[R36] 并发执行多个任务
来源：http://uzi.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bka.xinyue.icu

[R37] 把输出赋给变量
来源：http://ngy.yanxiufei.cn

files=$(ls -1)
来源：http://cuu.hesvh.cn

[R38] 管道串联
来源：http://vqx.snrcjt.cn

cat a.txt | grep -i error | wc -l
来源：http://bxv.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://mhj.redwolf501.top

cmd > out.log 2>&1
来源：http://gad.smart0.xyz

[R40] 追加写日志
来源：http://tcw.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://cyb.zhijiandao.cn

[R41] 丢弃输出
来源：http://iac.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://wez.jqgufenzy.top

[R42] 输入重定向
来源：http://zqr.yj20258888.top

wc -l < a.txt
来源：http://vms.gogol.net.cn

[R43] 按名字查找文件
来源：http://mno.iojbl.cn

find . -name "*.log" -type f
来源：http://gva.zdbjq.cn

[R44] 按修改时间查找
来源：http://jia.chenzaomai.com

find . -mtime -7 -type f
来源：http://lxg.guannengcc.top

[R45] 批量删除
来源：http://pwx.fzhhl.top

find . -name "*.tmp" -delete
来源：http://rdo.ydzc1.top

[R46] 递归替换文件内容
来源：http://cmh.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wtj.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://kov.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ddu.gzhubu.top

[R48] awk 取指定列
来源：http://uzg.sweek.top

awk '{print $1, $3}' a.txt
来源：http://vup.yuxming.cn

[R49] awk 带条件
来源：http://ore.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://efa.xziqi.cn

[R50] awk 求和
来源：http://fka.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://aeu.epnwcf.com

[R51] 排序去重取前几
来源：http://xgi.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hpq.shzxlz.cn

[R52] 统计行数
来源：http://lnl.gogol.net.cn

wc -l a.txt
来源：http://cpq.316326.xyz

[R53] 查看文件头与实时尾
来源：http://niz.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rkv.dashuyun.cn

[R54] 比较两个文件
来源：http://qqx.kuanghao11.cn

diff a.txt b.txt
来源：http://epi.feifeiyinyue.top

[R55] 压缩与解压
来源：http://jzg.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://imc.xuetiantiany.cn

[R56] 远程拷贝
来源：http://ezx.zdbjq.cn

scp file user@host:/path/
来源：http://agt.yangfankeji.com

[R57] 远程执行命令
来源：http://xvt.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://ujv.jinghuilouyu.cn

[R58] 下载文件
来源：http://xrt.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tfj.hesvh.cn

[R59] 发 POST JSON
来源：http://ugm.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://grt.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://aph.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://atw.ehwqpu.com

[R61] 磁盘占用
来源：http://ruf.pengpengdd.cyou

df -h;  du -sh *
来源：http://nyb.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://hip.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://tif.cdnleiting.top

[R63] 内存与进程
来源：http://hbf.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://aqu.zhixingplan.top

[R64] 结束进程
来源：http://dnf.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://qtn.hongshengwenyu.top

[R65] 查看端口占用
来源：http://bod.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://das.zhoulong.xyz

[R66] 定时任务
来源：http://irh.316326.xyz

crontab -e;  crontab -l
来源：http://asl.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://tpx.yongpay.top

openssl rand -hex 16
来源：http://snl.fktsv.cn

[R68] 计算文件校验值
来源：http://fil.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mqi.svipenyu.cn

[R69] 生成随机密码
来源：http://bjl.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://rps.xuanzx.com

[R70] 时间戳与互转
来源：http://bfn.sweek.top

date +%s;  date -d @1700000000
来源：http://hwn.yueranfly.top

[R71] 日期格式化
来源：http://snf.redwolf501.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zjr.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://ztf.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://phc.chenzaomai.com

[R73] 分割大日志
来源：http://olj.daria6918.cn

split -l 1000 big.log part_
来源：http://ksr.feifeiyinyue.top

[R74] 批量重命名
来源：http://nvj.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://piv.iojbl.cn

[R75] 导出环境变量
来源：http://goi.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://odw.aizwys.cn

[R76] 使用临时文件
来源：http://nak.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://thl.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://fph.pycfn.com

read -rp "请输入: " ans
来源：http://afx.hywenlv.cn

[R78] 交互式菜单
来源：http://wvz.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ooi.hammf.cn

[R79] 解析命令行选项
来源：http://fws.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fdc.yj202588.top

[R80] 查看脚本执行耗时
来源：http://wpx.yuanzhike.top

time ./run.sh
来源：http://xen.jyoumei.cn

================================================================================
来源：http://ovy.hysaishi.cn

S. C / C++ 专题
来源：http://upg.quarkkingdee.top

================================================================================
来源：http://hnm.kuanghao11.cn

[S01] C：Hello World
来源：http://yof.uphjek.com

#include <stdio.h>
来源：http://rbe.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qfp.meibo888.top

[S02] C：变量与格式化输出
来源：http://znt.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://ync.xziqi.cn

[S03] C：读入整数
来源：http://tcd.redwolf501.top

int x; scanf("%d", &x);
来源：http://ulh.ydjk.org.cn

[S04] C：字符串复制
来源：http://ooa.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://hty.316326.xyz

[S05] C：字符串长度
来源：http://ggg.jinqigfzy.top

strlen(s)
来源：http://jde.quarkkingdee.top

[S06] C：字符串比较
来源：http://gpg.cheryme.top

strcmp(a, b) == 0
来源：http://qhw.xziqi.cn

[S07] C：数组遍历求和
来源：http://uil.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://erk.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://hlu.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gjl.316326.xyz

[S09] C：结构体定义与初始化
来源：http://ttk.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oex.mhx1999.top

[S10] C：指针与解引用
来源：http://lot.aizwys.cn

int *p = &a;  *p = 5;
来源：http://xej.aizwys.cn

[S11] C：逐行读文件
来源：http://ugm.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://trb.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iyn.ivvv.top

fclose(f);
来源：http://jps.zhiwuduotai.top

[S12] C：写文件
来源：http://wgl.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://amr.hcnkem.com

[S13] C：宏定义
来源：http://qcq.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qfs.jinghuilouyu.cn

[S14] C：枚举
来源：http://zzi.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://zwl.sweek.top

[S15] C：类型转换
来源：http://efo.feifeiyinyue.top

(double) a / b
来源：http://epa.feifeiyinyue.top

[S16] C：位操作置位
来源：http://afc.xuanzx.com

x |= (1 << 3);
来源：http://olv.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://jsy.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kgt.shangyingyoupin.top

[S18] C：命令行参数
来源：http://uss.meibo888.top

int main(int argc, char **argv)
来源：http://ffh.quarkkingdee.top

[S19] C：快速排序
来源：http://dlc.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://atg.jinqigufen.top

[S20] C：二分查找
来源：http://fpy.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://efs.wangdashe.top

[S21] C：字符类别判断
来源：http://tbp.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mpd.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://vgt.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mju.zhengqikj.top

[S23] C：随机数
来源：http://afi.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jrk.52xcode.cn

[S24] C：获取本地时间
来源：http://hco.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dev.kuanghao11.cn

[S25] C：内存拷贝
来源：http://juk.smart0.xyz

memcpy(dst, src, n);
来源：http://mcc.zycfv.cn

[S26] C：内存清零
来源：http://onf.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://wkh.uphjek.com

[S27] C：定义常量
来源：http://taa.hcnkem.com

const double PI = 3.14159;
来源：http://soi.gaohongyu789.top

[S28] C：静态变量
来源：http://gey.xziqi.cn

static int counter = 0;
来源：http://xmk.epnwcf.com

[S29] C：变参函数
来源：http://kcn.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rll.jinqigfzy.top

[S30] C：头文件保护
来源：http://ubv.zycfv.cn

#ifndef X_H
来源：http://xba.ywan-chungtsiang.top

#define X_H
来源：http://luh.ehwqpu.com

#endif
来源：http://qlj.fzhhl.top

[S31] C++：Hello World
来源：http://yow.bbcook.cn

#include <iostream>
来源：http://noj.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://xzg.xziqi.cn

[S32] C++：字符串
来源：http://tpf.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://ojy.fzhhl.top

[S33] C++：vector 增删
来源：http://ege.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rhj.cdnleiting.top

[S34] C++：遍历 vector
来源：http://mbz.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://vlh.jianghu66.top

[S35] C++：map
来源：http://zho.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jcp.yuxming.cn

[S36] C++：unordered_map
来源：http://xty.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kfe.dianchejie.cn

[S37] C++：set
来源：http://evw.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lcs.wangdashe.top

[S38] C++：排序
来源：http://lzp.cheryme.top

std::sort(v.begin(), v.end());
来源：http://tkw.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://qfz.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rnl.sxryk.cn

[S40] C++：查找元素
来源：http://sea.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xvh.wangdashe.top

[S41] C++：类与构造函数
来源：http://kun.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tax.yvedp.cn

[S42] C++：继承与虚函数
来源：http://rbu.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://qha.hysaishi.cn

[S43] C++：智能指针
来源：http://aiz.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://hqj.ctjpmb.com

[S44] C++：引用传参
来源：http://obi.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://zgb.tanke756.top

[S45] C++：lambda
来源：http://shl.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://nuz.daria6918.cn

[S46] C++：函数模板
来源：http://ihz.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zfm.yj20258.top


<!-- 参考信息 -->