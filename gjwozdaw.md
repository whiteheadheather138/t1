代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://osn.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://miu.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ppx.cashguo.top

[Q57] 行号
来源：http://yna.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://drv.shangyingyoupin.top

[Q58] 累计求和
来源：http://yay.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vjd.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://aaq.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wwk.jinghuilouyu.cn

[Q60] 取上一行 / 下一行
来源：http://ckd.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ozr.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://azj.316326.xyz

[Q61] 移动平均
来源：http://uba.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iys.zhoulong.xyz

[Q62] 分组占比
来源：http://arl.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ncc.shuidangran.top

[Q63] 开启事务
来源：http://ifi.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uva.yj20258.top

[Q64] 提交事务
来源：http://eil.jlsjyb.cn

COMMIT;
来源：http://bid.316326.xyz

[Q65] 回滚事务
来源：http://ekh.hammf.cn

ROLLBACK;
来源：http://fwq.hfpthk.cn

[Q66] 行锁查询
来源：http://evt.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qvc.wangdashe.top

[Q67] 设置隔离级别
来源：http://kha.gaohongyu789.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jqt.yueranfly.top

[Q68] 保存点
来源：http://ssz.tanke756.top

SAVEPOINT sp1;
来源：http://rdv.daria6918.cn

ROLLBACK TO sp1;
来源：http://jkt.ctjpmb.com

[Q69] 查看执行计划
来源：http://ixz.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hhl.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://xom.jyoumei.cn

ANALYZE TABLE users;
来源：http://mwj.zhijiandao.cn

[Q71] 查看建表语句
来源：http://qia.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hoc.hongshengwenyu.top

[Q72] 查看索引
来源：http://nru.nwbrower.top

SHOW INDEX FROM users;
来源：http://jdq.havefunace.top

[Q73] 查看表状态
来源：http://khw.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://aeo.fehbvm.com

[Q74] 强制使用索引
来源：http://eyn.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iqa.pycfn.com

[Q75] 日期格式化
来源：http://dhs.gogol.net.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yul.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fdo.ehwqpu.com

[Q76] 按天统计
来源：http://qdm.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://keh.xinyue.icu

[Q77] 时间加减
来源：http://mbj.cucudq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://voi.guannengcc.top

[Q78] 当前时间
来源：http://kpe.yj20258.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pix.nanxinkj.top

[Q79] 字符串拼接
来源：http://iao.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pef.pengpengdd.cyou

[Q80] 字符串截取
来源：http://tji.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iqz.yangfankeji.com

[Q81] 字符串替换
来源：http://fzu.sxryk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tlu.daxiang520.top

[Q82] 字符长度与字节长度
来源：http://gab.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://soz.haohaochexian.top

[Q83] 大小写转换
来源：http://pvj.shzxlz.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oxc.daria6918.cn

[Q84] 去除首尾空格
来源：http://orh.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://npg.shanyushiyangtech.top

[Q85] 数值取整
来源：http://tdc.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wfj.svipenyu.cn

[Q86] 读取 JSON 字段
来源：http://zdh.chenzaomai.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ags.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://duv.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blb.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://bdy.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uet.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ffv.yfazqb.com

[Q89] 判断表是否存在
来源：http://ojr.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rzm.zdqjudy.top

[Q90] 生成序号列
来源：http://hxb.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://chw.zhijiandao.cn

================================================================================
来源：http://uqf.snrcjt.cn

R. Bash 专题
来源：http://izb.cashguo.top

================================================================================
来源：http://dca.hfpthk.cn

[R01] shebang 与严格模式
来源：http://kjg.cqqwz.cn

#!/usr/bin/env bash
来源：http://xxl.yanxiufei.cn

set -euo pipefail
来源：http://qju.zhoulong.xyz

[R02] 变量赋值与使用
来源：http://wlr.0kj1m.cn

name="Tom"; echo "$name"
来源：http://bgs.tarul.cn

[R03] 只读变量
来源：http://cas.hammf.cn

readonly PI=3.14
来源：http://ysr.zhijiandao.cn

[R04] 位置参数
来源：http://adm.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://khr.hcnkem.com

[R05] 参数默认值
来源：http://eyw.dianchejie.cn

name="${1:-default}"
来源：http://htu.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://xgz.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ekv.xinyue.icu

[R07] if 判断文件
来源：http://vvk.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dit.dashuyun.cn

[R08] 数值比较
来源：http://nuf.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pxc.hongshengwenyu.top

[R09] 字符串比较
来源：http://kur.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hik.jqgufenzy.top

[R10] 正则匹配
来源：http://iwn.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ujd.ydzc1.top

[R11] case 多分支
来源：http://yrw.vehdjk.com

case "$1" in
来源：http://gyr.gogol.net.cn

start) echo "启动" ;;
来源：http://prk.zdqjudy.top

stop)  echo "停止" ;;
来源：http://nyt.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://zxo.yueranfly.top

esac
来源：http://ejd.yanxiufei.cn

[R12] for 遍历文件
来源：http://yel.gotoacloud.top

for f in *.txt; do echo "$f"; done
来源：http://hhf.c1oappe.top

[R13] for 计数循环
来源：http://ueg.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://frf.vehdjk.com

[R14] C 风格 for
来源：http://klh.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tfd.sysykeji.top

[R15] while 逐行读文件
来源：http://apt.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kih.0kj1m.cn

[R16] until 等待条件
来源：http://eyp.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zpl.yuxming.cn

[R17] 数组定义与取值
来源：http://gai.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://zkk.tian-w.cn

[R18] 遍历数组
来源：http://owv.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://axr.ybcxt.top

[R19] 数组长度
来源：http://qbu.zhengqikj.top

echo "${#arr[@]}"
来源：http://pah.jyoumei.cn

[R20] 关联数组（字典）
来源：http://jly.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://olr.zdqjudy.top

[R21] 字符串长度
来源：http://ksb.gzhubu.top

echo "${#s}"
来源：http://nso.c1oappe.top

[R22] 截取子串
来源：http://jrk.hammf.cn

echo "${s:0:5}"
来源：http://fxc.jiagoushi.top

[R23] 字符串替换
来源：http://tlb.iojbl.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ljj.xylfe.cn

[R24] 大小写转换
来源：http://vvw.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://hrd.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://sgq.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dbb.vqdsnc.cn

[R26] 命令替换
来源：http://ikl.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://fqt.cashguo.top

[R27] 算术展开
来源：http://aik.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://jza.fengsongda.top

[R28] 浮点运算
来源：http://zvu.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://imz.shanyushiyangkeji.top

[R29] 定义函数
来源：http://cie.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ijm.gotoacloud.top

[R30] 函数返回状态码
来源：http://rsi.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://lca.zhijiandao.cn

[R31] 局部变量
来源：http://tub.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://hpc.hfpthk.cn

[R32] 参数个数校验
来源：http://cdn.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tbp.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://xlx.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ebv.ybcxt.top

[R34] 退出时清理
来源：http://lgp.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://ajc.daxiang520.top

[R35] 后台执行并等待
来源：http://yls.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tji.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://agb.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tik.zycfv.cn

[R37] 把输出赋给变量
来源：http://oql.redwolf501.top

files=$(ls -1)
来源：http://mtv.fanxiaobao.xyz

[R38] 管道串联
来源：http://cnf.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://rwj.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://tke.9152youxi.cn

cmd > out.log 2>&1
来源：http://rja.yvedp.cn

[R40] 追加写日志
来源：http://xtz.pycfn.com

echo "log" >> out.log
来源：http://ndm.sweek.top

[R41] 丢弃输出
来源：http://siw.ybcxt.top

cmd >/dev/null 2>&1
来源：http://dct.shzxlz.cn

[R42] 输入重定向
来源：http://bru.ivvv.top

wc -l < a.txt
来源：http://oqk.gogol.net.cn

[R43] 按名字查找文件
来源：http://khr.sjlbkw.cn

find . -name "*.log" -type f
来源：http://ghl.nanxuanxn.top

[R44] 按修改时间查找
来源：http://wfl.sweek.top

find . -mtime -7 -type f
来源：http://tek.ehwqpu.com

[R45] 批量删除
来源：http://eaz.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://seh.pycfn.com

[R46] 递归替换文件内容
来源：http://ymu.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dzc.birdmap.top

[R47] sed 单行替换
来源：http://cwg.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://new.jyoumei.cn

[R48] awk 取指定列
来源：http://tym.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://qyv.xylfe.cn

[R49] awk 带条件
来源：http://zkq.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jco.jqgufenzy.top

[R50] awk 求和
来源：http://stb.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://itj.yj20258888.top

[R51] 排序去重取前几
来源：http://olc.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bec.nanxinkj.top

[R52] 统计行数
来源：http://uhk.sjlbkw.cn

wc -l a.txt
来源：http://tzq.meibo888.top

[R53] 查看文件头与实时尾
来源：http://ctw.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ywc.wangshuangyany.cn

[R54] 比较两个文件
来源：http://bua.pengpengdd.cyou

diff a.txt b.txt
来源：http://zup.zhongyouzk.top

[R55] 压缩与解压
来源：http://lrz.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kxw.52xcode.cn

[R56] 远程拷贝
来源：http://lkm.yangfankeji.com

scp file user@host:/path/
来源：http://aid.xuetiantiany.cn

[R57] 远程执行命令
来源：http://vvn.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://zdk.zhoulong.xyz

[R58] 下载文件
来源：http://vzf.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wxy.yfazqb.com

[R59] 发 POST JSON
来源：http://hhv.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kqg.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://fve.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pjv.tian-w.cn

[R61] 磁盘占用
来源：http://flb.shzxlz.cn

df -h;  du -sh *
来源：http://pmx.smart0.xyz

[R62] 找最占空间的文件
来源：http://tkr.ivvv.top

du -ah . | sort -rh | head -10
来源：http://qpm.cucudq.cn

[R63] 内存与进程
来源：http://kjo.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://yua.nanxinkj.top

[R64] 结束进程
来源：http://qwe.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://pwc.yongpay.top

[R65] 查看端口占用
来源：http://hjg.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zbx.gotoacloud.top

[R66] 定时任务
来源：http://dem.vehdjk.com

crontab -e;  crontab -l
来源：http://hib.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://ayf.fktsv.cn

openssl rand -hex 16
来源：http://cma.svipenyu.cn

[R68] 计算文件校验值
来源：http://obz.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://erp.zhoulong.xyz

[R69] 生成随机密码
来源：http://hpk.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://enp.jyoumei.cn

[R70] 时间戳与互转
来源：http://osn.tian-w.cn

date +%s;  date -d @1700000000
来源：http://wqy.jiagoushi.top

[R71] 日期格式化
来源：http://tpe.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cgy.hfpthk.cn

[R72] 等待端口就绪
来源：http://yqi.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://icf.yuanzhike.top

[R73] 分割大日志
来源：http://zkq.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://rap.daria6918.cn

[R74] 批量重命名
来源：http://nss.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uvt.jiagoushi.top

[R75] 导出环境变量
来源：http://jmn.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://ltr.yueranfly.top

[R76] 使用临时文件
来源：http://vqi.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ueo.jlsjyb.cn

[R77] 读取用户输入
来源：http://uum.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://nwx.xuetiantiany.cn

[R78] 交互式菜单
来源：http://pbs.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://flo.yonumen.top

[R79] 解析命令行选项
来源：http://wua.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vwk.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://syk.xziqi.cn

time ./run.sh
来源：http://ppw.zhiwuduotai.top

================================================================================
来源：http://qqz.jlsjyb.cn

S. C / C++ 专题
来源：http://qhk.c1oappe.top

================================================================================
来源：http://hcu.zdqjudy.top

[S01] C：Hello World
来源：http://gjf.mhx1999.top

#include <stdio.h>
来源：http://eji.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xhv.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://kqo.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://kaa.chenlongwang.top

[S03] C：读入整数
来源：http://xge.ydzc1.top

int x; scanf("%d", &x);
来源：http://qna.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://lgv.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ddw.yueranfly.top

[S05] C：字符串长度
来源：http://xjj.kuanghao11.cn

strlen(s)
来源：http://rqn.hammf.cn

[S06] C：字符串比较
来源：http://kac.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://fsg.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://rkc.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bvf.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://eid.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://arr.ivvv.top

[S09] C：结构体定义与初始化
来源：http://yvu.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qbd.xuanzx.com

[S10] C：指针与解引用
来源：http://wlh.xinyue.icu

int *p = &a;  *p = 5;
来源：http://mqa.vqdsnc.cn

[S11] C：逐行读文件
来源：http://pef.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ajg.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gbc.hesvh.cn

fclose(f);
来源：http://twp.gogol.net.cn

[S12] C：写文件
来源：http://cco.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xfl.yonumen.top

[S13] C：宏定义
来源：http://rrq.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bxb.feifeiyinyue.top

[S14] C：枚举
来源：http://ujg.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://tct.chenlongwang.top

[S15] C：类型转换
来源：http://htz.9152youxi.cn

(double) a / b
来源：http://ajm.uphjek.com

[S16] C：位操作置位
来源：http://ctz.jqgfzy.top

x |= (1 << 3);
来源：http://ymm.vehdjk.com

[S17] C：安全拼接字符串
来源：http://uvt.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jmd.dashuyun.cn

[S18] C：命令行参数
来源：http://hlr.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://oni.yongpay.top

[S19] C：快速排序
来源：http://rsh.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lbv.daria6918.cn

[S20] C：二分查找
来源：http://zle.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wqg.ppjwa.cn

[S21] C：字符类别判断
来源：http://psl.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aku.cqqwz.cn

[S22] C：字符串转数字
来源：http://ntk.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://ori.aizwys.cn

[S23] C：随机数
来源：http://fzl.cdnleiting.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jvw.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://tdg.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://okq.quarkkingdee.top

[S25] C：内存拷贝
来源：http://jmg.xziqi.cn

memcpy(dst, src, n);
来源：http://mzy.ydjk.org.cn

[S26] C：内存清零
来源：http://jxz.ppjwa.cn


<!-- 参考信息 -->