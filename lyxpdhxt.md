代发 wailian999

[Q65] 回滚事务
来源：http://ake.yj20258.top

ROLLBACK;
来源：http://kgy.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://zqx.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://whu.birdmap.top

[Q67] 设置隔离级别
来源：http://dha.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hsn.guannengcc.top

[Q68] 保存点
来源：http://zxu.vqdsnc.cn

SAVEPOINT sp1;
来源：http://xww.zdqjudy.top

ROLLBACK TO sp1;
来源：http://ior.hfpthk.cn

[Q69] 查看执行计划
来源：http://mmn.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dvk.ybcxt.top

[Q70] 更新统计信息
来源：http://agu.xuanzx.com

ANALYZE TABLE users;
来源：http://dil.kuanghao11.cn

[Q71] 查看建表语句
来源：http://ryc.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dhe.sxryk.cn

[Q72] 查看索引
来源：http://wqs.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://jsl.tian-w.cn

[Q73] 查看表状态
来源：http://duy.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://slq.ppjwa.cn

[Q74] 强制使用索引
来源：http://lzy.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uft.haohaochexian.top

[Q75] 日期格式化
来源：http://mfb.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xgd.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://txh.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://byo.ybcxt.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fbu.aibaodan.cn

[Q77] 时间加减
来源：http://yly.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fua.316326.xyz

[Q78] 当前时间
来源：http://rca.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cka.yongpay.top

[Q79] 字符串拼接
来源：http://xfq.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fqx.tarul.cn

[Q80] 字符串截取
来源：http://ezi.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://czt.zhijiandao.cn

[Q81] 字符串替换
来源：http://wpj.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://udx.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://jte.316326.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ged.ctjpmb.com

[Q83] 大小写转换
来源：http://wgh.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uap.xuanzx.com

[Q84] 去除首尾空格
来源：http://owm.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://smi.hnqzz.top

[Q85] 数值取整
来源：http://gmu.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fvm.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://kvm.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rel.yuxming.cn

[Q87] JSON 字段做条件
来源：http://jxg.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xwq.hywenlv.cn

[Q88] 行转列（条件聚合）
来源：http://kgh.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ltk.aizwys.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oah.shzxlz.cn

[Q89] 判断表是否存在
来源：http://zke.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bql.c1oappe.top

[Q90] 生成序号列
来源：http://xyw.chenzaomai.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vtx.ydjk.org.cn

================================================================================
来源：http://jtq.0kj1m.cn

R. Bash 专题
来源：http://xei.ctjpmb.com

================================================================================
来源：http://yxt.yongpay.top

[R01] shebang 与严格模式
来源：http://vyp.dashuyun.cn

#!/usr/bin/env bash
来源：http://pmg.nwbrower.top

set -euo pipefail
来源：http://fzc.shzxlz.cn

[R02] 变量赋值与使用
来源：http://olg.xuanzx.com

name="Tom"; echo "$name"
来源：http://gig.smart0.xyz

[R03] 只读变量
来源：http://hyl.cdnleiting.top

readonly PI=3.14
来源：http://glf.svipenyu.cn

[R04] 位置参数
来源：http://heg.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oet.sweek.top

[R05] 参数默认值
来源：http://uuf.nanxuanxn.top

name="${1:-default}"
来源：http://ryu.hnqzz.top

[R06] 判断命令是否存在
来源：http://soj.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wom.chenjidiqi.icu

[R07] if 判断文件
来源：http://xgn.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eqt.svipenyu.cn

[R08] 数值比较
来源：http://hao.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://ihm.daxiang520.top

[R09] 字符串比较
来源：http://knx.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xuj.yongpay.top

[R10] 正则匹配
来源：http://rai.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uzr.yonumen.top

[R11] case 多分支
来源：http://cyl.mhx1999.top

case "$1" in
来源：http://jtb.cashguo.top

start) echo "启动" ;;
来源：http://ykq.fengsongda.top

stop)  echo "停止" ;;
来源：http://ryv.ydjk.org.cn

*)     echo "未知命令" ;;
来源：http://vxh.zhengqikj.top

esac
来源：http://bpy.hcnkem.com

[R12] for 遍历文件
来源：http://idz.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://phg.yuanzhike.top

[R13] for 计数循环
来源：http://tcx.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://imq.cqqwz.cn

[R14] C 风格 for
来源：http://jsp.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oea.daria6918.cn

[R15] while 逐行读文件
来源：http://ocu.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fen.tanke756.top

[R16] until 等待条件
来源：http://omr.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lra.jiagoushi.top

[R17] 数组定义与取值
来源：http://svx.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://juc.316326.xyz

[R18] 遍历数组
来源：http://gnh.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dbq.xuanzx.com

[R19] 数组长度
来源：http://uyg.yonumen.top

echo "${#arr[@]}"
来源：http://ezz.wangdashe.top

[R20] 关联数组（字典）
来源：http://ywc.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qlw.snrcjt.cn

[R21] 字符串长度
来源：http://myl.jqgufenzy.top

echo "${#s}"
来源：http://rvj.yuanzhike.top

[R22] 截取子串
来源：http://mwx.pycfn.com

echo "${s:0:5}"
来源：http://aki.c1oappe.top

[R23] 字符串替换
来源：http://yhh.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nxe.nanxuanxn.top

[R24] 大小写转换
来源：http://ndn.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yyk.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://bbv.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wov.vehdjk.com

[R26] 命令替换
来源：http://kfg.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://qda.tarul.cn

[R27] 算术展开
来源：http://dbj.nwbrower.top

echo $((1 + 2 * 3))
来源：http://wgi.ybcxt.top

[R28] 浮点运算
来源：http://twx.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://yqm.jinqigfzy.top

[R29] 定义函数
来源：http://emi.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://puk.zhijiandao.cn

[R30] 函数返回状态码
来源：http://knx.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://tdc.jlsjyb.cn

[R31] 局部变量
来源：http://yec.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://tps.yangfankeji.com

[R32] 参数个数校验
来源：http://pwg.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rqx.havefunace.top

[R33] 捕获错误并提示行号
来源：http://vmk.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://udb.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://dml.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ozc.ctjpmb.com

[R35] 后台执行并等待
来源：http://bmc.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://inw.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://fuk.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qwo.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://npa.cdnleiting.top

files=$(ls -1)
来源：http://hpy.aizwys.cn

[R38] 管道串联
来源：http://jex.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://ria.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://iaq.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://xwg.xuetiantiany.cn

[R40] 追加写日志
来源：http://aht.hammf.cn

echo "log" >> out.log
来源：http://dab.daxiang520.top

[R41] 丢弃输出
来源：http://ggh.jyoumei.cn

cmd >/dev/null 2>&1
来源：http://kdq.xziqi.cn

[R42] 输入重定向
来源：http://lwu.cqqwz.cn

wc -l < a.txt
来源：http://xkk.zdbjq.cn

[R43] 按名字查找文件
来源：http://ubf.jinqigfzy.top

find . -name "*.log" -type f
来源：http://wll.mhx1999.top

[R44] 按修改时间查找
来源：http://mzh.aibaodan.cn

find . -mtime -7 -type f
来源：http://asy.ywan-chungtsiang.top

[R45] 批量删除
来源：http://dzt.jianghu66.top

find . -name "*.tmp" -delete
来源：http://tye.yj20258888.top

[R46] 递归替换文件内容
来源：http://drt.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bej.cqqwz.cn

[R47] sed 单行替换
来源：http://hag.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nvu.tarul.cn

[R48] awk 取指定列
来源：http://amx.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://jxo.xuetiantiany.cn

[R49] awk 带条件
来源：http://ywn.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vzf.sufxvd.cn

[R50] awk 求和
来源：http://qxk.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://uvm.havefunace.top

[R51] 排序去重取前几
来源：http://osm.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mlx.ivvv.top

[R52] 统计行数
来源：http://nlj.jqgufenzy.top

wc -l a.txt
来源：http://cff.yangfankeji.com

[R53] 查看文件头与实时尾
来源：http://qsj.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mnu.dashuyun.cn

[R54] 比较两个文件
来源：http://yav.guowangkeji.top

diff a.txt b.txt
来源：http://rcm.xuanzx.com

[R55] 压缩与解压
来源：http://qjo.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jce.svipenyu.cn

[R56] 远程拷贝
来源：http://mjg.yj20258.top

scp file user@host:/path/
来源：http://lmt.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://bov.cucudq.cn

ssh user@host 'uptime'
来源：http://stm.xylfe.cn

[R58] 下载文件
来源：http://xzy.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wxg.hammf.cn

[R59] 发 POST JSON
来源：http://xko.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vtq.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://fkn.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zbt.uphjek.com

[R61] 磁盘占用
来源：http://mbv.jinqigfzy.top

df -h;  du -sh *
来源：http://ygr.tarul.cn

[R62] 找最占空间的文件
来源：http://zor.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://nel.yj202588.top

[R63] 内存与进程
来源：http://sdj.fengsongda.top

free -h;  ps aux | grep nginx
来源：http://eeu.cqqwz.cn

[R64] 结束进程
来源：http://vvu.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://spe.jinqigufen.top

[R65] 查看端口占用
来源：http://fpp.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ogb.jinghuilouyu.cn

[R66] 定时任务
来源：http://dym.hnqzz.top

crontab -e;  crontab -l
来源：http://mxr.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://fmg.ehwqpu.com

openssl rand -hex 16
来源：http://ioe.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://hvz.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tdm.shuidangran.top

[R69] 生成随机密码
来源：http://zyb.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://evu.chenlongwang.top

[R70] 时间戳与互转
来源：http://haa.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://snn.jinqigfzy.top

[R71] 日期格式化
来源：http://eua.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wwx.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://uim.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uhd.jiagoushi.top

[R73] 分割大日志
来源：http://nti.zycfv.cn

split -l 1000 big.log part_
来源：http://pvr.gzhubu.top

[R74] 批量重命名
来源：http://yqu.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kne.0kj1m.cn

[R75] 导出环境变量
来源：http://qsa.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://gpd.0kj1m.cn

[R76] 使用临时文件
来源：http://fca.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ovd.52xcode.cn

[R77] 读取用户输入
来源：http://ffu.daria6918.cn

read -rp "请输入: " ans
来源：http://vwu.wangdashe.top

[R78] 交互式菜单
来源：http://imk.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://aqt.cheryme.top

[R79] 解析命令行选项
来源：http://drk.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ttr.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://fvt.guowangkeji.top

time ./run.sh
来源：http://bkh.0kj1m.cn

================================================================================
来源：http://gif.yueranfly.top

S. C / C++ 专题
来源：http://wdf.nanxinkj.top

================================================================================
来源：http://rcl.cqqwz.cn

[S01] C：Hello World
来源：http://jum.bbcook.cn

#include <stdio.h>
来源：http://rqs.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vtf.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://sgr.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://tag.zhengqikj.top

[S03] C：读入整数
来源：http://scx.iojbl.cn

int x; scanf("%d", &x);
来源：http://oct.mhx1999.top

[S04] C：字符串复制
来源：http://lah.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://roa.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://ybj.wangshuangyany.cn

strlen(s)
来源：http://vmx.hnxiangtu.top

[S06] C：字符串比较
来源：http://zfh.zhoulong.xyz

strcmp(a, b) == 0
来源：http://bvj.yueranfly.top

[S07] C：数组遍历求和
来源：http://nhd.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ybe.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://rwb.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ecf.xuetiantiany.cn

[S09] C：结构体定义与初始化
来源：http://jwh.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vdu.yj20258.top

[S10] C：指针与解引用
来源：http://ezv.havefunace.top

int *p = &a;  *p = 5;
来源：http://fny.ppjwa.cn

[S11] C：逐行读文件
来源：http://qbs.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://jjc.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xab.meibo888.top

fclose(f);
来源：http://mii.sjlbkw.cn

[S12] C：写文件
来源：http://qfw.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eqq.uphjek.com

[S13] C：宏定义
来源：http://vgv.sufxvd.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://siy.uphjek.com

[S14] C：枚举
来源：http://uop.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://xil.ivvv.top

[S15] C：类型转换
来源：http://mjf.gotoacloud.top

(double) a / b
来源：http://jgw.smart0.xyz

[S16] C：位操作置位
来源：http://ybv.shzxlz.cn

x |= (1 << 3);
来源：http://fdj.iojbl.cn

[S17] C：安全拼接字符串
来源：http://gic.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nwf.tarul.cn

[S18] C：命令行参数
来源：http://xdv.zhoulong.xyz

int main(int argc, char **argv)
来源：http://esq.tanke756.top

[S19] C：快速排序
来源：http://itr.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://enf.zhiwuduotai.top

[S20] C：二分查找
来源：http://ojp.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uwz.zdbjq.cn

[S21] C：字符类别判断
来源：http://fro.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cwy.iojbl.cn

[S22] C：字符串转数字
来源：http://ecq.nanxinkj.top

atoi("42");  strtod("3.14", NULL);
来源：http://ylx.zhiwuduotai.top

[S23] C：随机数
来源：http://ide.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ayz.wangdashe.top

[S24] C：获取本地时间
来源：http://jug.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://flt.cdnleiting.top

[S25] C：内存拷贝
来源：http://mmn.dashuyun.cn

memcpy(dst, src, n);
来源：http://ipd.shzxlz.cn

[S26] C：内存清零
来源：http://dql.iojbl.cn

memset(a, 0, sizeof a);
来源：http://xtf.jqgufenzy.top

[S27] C：定义常量
来源：http://pnu.aibaodan.cn

const double PI = 3.14159;
来源：http://mtl.bbcook.cn

[S28] C：静态变量
来源：http://nym.tian-w.cn

static int counter = 0;
来源：http://zfy.zycfv.cn

[S29] C：变参函数
来源：http://zpl.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eeo.ehwqpu.com

[S30] C：头文件保护
来源：http://aey.zdbjq.cn

#ifndef X_H
来源：http://bsq.yj202588.top

#define X_H
来源：http://she.epnwcf.com

#endif
来源：http://cqw.meibo888.top

[S31] C++：Hello World
来源：http://jvn.xuetiantiany.cn

#include <iostream>
来源：http://huj.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://ggf.ydjk.org.cn

[S32] C++：字符串
来源：http://qat.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://jfi.gaohongyu789.top

[S33] C++：vector 增删
来源：http://smm.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qmc.nwbrower.top

[S34] C++：遍历 vector
来源：http://mpx.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://yiz.zhengqikj.top


<!-- 参考信息 -->