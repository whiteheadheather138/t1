代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mvo.ivvv.top

[Q54] 清空表
来源：http://mfk.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://ysx.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://tvs.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cmr.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://szx.aibaodan.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://efn.sxryk.cn

[Q57] 行号
来源：http://ysy.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://awi.daxiang520.top

[Q58] 累计求和
来源：http://wxy.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ych.jyoumei.cn

[Q59] 分组内累计
来源：http://nbq.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://abg.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://mxj.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jyl.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gfg.fktsv.cn

[Q61] 移动平均
来源：http://oqd.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qbb.cucudq.cn

[Q62] 分组占比
来源：http://vek.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ejl.zycfv.cn

[Q63] 开启事务
来源：http://uqd.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://rjt.gotoacloud.top

[Q64] 提交事务
来源：http://fjm.iojbl.cn

COMMIT;
来源：http://eva.dianchejie.cn

[Q65] 回滚事务
来源：http://lrw.snrcjt.cn

ROLLBACK;
来源：http://ugb.fktsv.cn

[Q66] 行锁查询
来源：http://ydz.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ysx.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://wpk.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aki.jianghu66.top

[Q68] 保存点
来源：http://mjb.nanxuanxn.top

SAVEPOINT sp1;
来源：http://lim.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://smo.0kj1m.cn

[Q69] 查看执行计划
来源：http://sjv.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sqw.kuanghao11.cn

[Q70] 更新统计信息
来源：http://vko.tanke756.top

ANALYZE TABLE users;
来源：http://mzs.9152youxi.cn

[Q71] 查看建表语句
来源：http://grf.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gnr.sxryk.cn

[Q72] 查看索引
来源：http://pfy.sysykeji.top

SHOW INDEX FROM users;
来源：http://ege.yongpay.top

[Q73] 查看表状态
来源：http://tse.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nho.snrcjt.cn

[Q74] 强制使用索引
来源：http://zgn.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rnq.fktsv.cn

[Q75] 日期格式化
来源：http://tbi.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oha.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vuc.yj20258888.top

[Q76] 按天统计
来源：http://asg.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://clx.bjfxy.top

[Q77] 时间加减
来源：http://hne.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dcj.sjlbkw.cn

[Q78] 当前时间
来源：http://ore.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zey.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://yvn.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cha.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://rin.hesvh.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nid.yanxiufei.cn

[Q81] 字符串替换
来源：http://isw.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oni.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://wep.zhoulong.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mdi.tianlin.xyz

[Q83] 大小写转换
来源：http://vbf.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hmu.shuidangran.top

[Q84] 去除首尾空格
来源：http://kgh.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://bvy.hywenlv.cn

[Q85] 数值取整
来源：http://qdf.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uat.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://wym.vqdsnc.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blc.daxiang520.top

[Q87] JSON 字段做条件
来源：http://smr.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://njo.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://dsi.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://esb.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pmp.hcnkem.com

[Q89] 判断表是否存在
来源：http://lyn.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hqu.cdnleiting.top

[Q90] 生成序号列
来源：http://ikr.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hxh.jinqigfzy.top

================================================================================
来源：http://gtz.xuanzx.com

R. Bash 专题
来源：http://fpn.xinyue.icu

================================================================================
来源：http://lsm.xylfe.cn

[R01] shebang 与严格模式
来源：http://ppp.quarkkingdee.top

#!/usr/bin/env bash
来源：http://hjh.zhoulong.xyz

set -euo pipefail
来源：http://piz.yj20258888.top

[R02] 变量赋值与使用
来源：http://jll.ppjwa.cn

name="Tom"; echo "$name"
来源：http://qqw.pycfn.com

[R03] 只读变量
来源：http://pav.jinyuanbaomall.cn

readonly PI=3.14
来源：http://mzs.yj202588.top

[R04] 位置参数
来源：http://nug.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dol.yj202588.top

[R05] 参数默认值
来源：http://tdj.yfazqb.com

name="${1:-default}"
来源：http://foo.ctjpmb.com

[R06] 判断命令是否存在
来源：http://jpv.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qug.yueranfly.top

[R07] if 判断文件
来源：http://rdh.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tmu.vqdsnc.cn

[R08] 数值比较
来源：http://edv.hywenlv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ngy.hcnkem.com

[R09] 字符串比较
来源：http://lzp.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pax.iojbl.cn

[R10] 正则匹配
来源：http://qlt.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://opb.ctjpmb.com

[R11] case 多分支
来源：http://yjn.epnwcf.com

case "$1" in
来源：http://dre.hnxiangtu.top

start) echo "启动" ;;
来源：http://hfw.smart0.xyz

stop)  echo "停止" ;;
来源：http://irt.hnxiangtu.top

*)     echo "未知命令" ;;
来源：http://npe.cucudq.cn

esac
来源：http://ldv.xuetiantiany.cn

[R12] for 遍历文件
来源：http://wtf.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://ret.nanxuanxn.top

[R13] for 计数循环
来源：http://gsg.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://kmo.cheryme.top

[R14] C 风格 for
来源：http://rse.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qvq.jqgufenzy.top

[R15] while 逐行读文件
来源：http://ydh.tanke756.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cpp.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://zcw.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ktv.yangfankeji.com

[R17] 数组定义与取值
来源：http://emu.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://oik.chenjidiqi.icu

[R18] 遍历数组
来源：http://bwn.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nsd.pycfn.com

[R19] 数组长度
来源：http://ppn.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://sor.redwolf501.top

[R20] 关联数组（字典）
来源：http://vix.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sfe.bjfxy.top

[R21] 字符串长度
来源：http://qxl.sxryk.cn

echo "${#s}"
来源：http://ptn.fanxiaobao.xyz

[R22] 截取子串
来源：http://nzx.ydjk.org.cn

echo "${s:0:5}"
来源：http://asl.jyoumei.cn

[R23] 字符串替换
来源：http://jjw.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pad.wangdashe.top

[R24] 大小写转换
来源：http://jny.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://orc.xingfuxueyuan.xyz

[R25] 去后缀 / 去前缀
来源：http://oke.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ivn.bbcook.cn

[R26] 命令替换
来源：http://psg.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://dlm.ehwqpu.com

[R27] 算术展开
来源：http://qgq.yj20258888.top

echo $((1 + 2 * 3))
来源：http://rfy.hywenlv.cn

[R28] 浮点运算
来源：http://lsh.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://fji.hammf.cn

[R29] 定义函数
来源：http://urp.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ybq.xuanzx.com

[R30] 函数返回状态码
来源：http://wqz.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://snv.birdmap.top

[R31] 局部变量
来源：http://xbj.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://xar.hfpthk.cn

[R32] 参数个数校验
来源：http://cfx.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jnb.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://kyo.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ahz.haohaochexian.top

[R34] 退出时清理
来源：http://yde.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xkj.pycfn.com

[R35] 后台执行并等待
来源：http://won.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sxy.ybcxt.top

[R36] 并发执行多个任务
来源：http://ayq.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://puq.316326.xyz

[R37] 把输出赋给变量
来源：http://phu.52xcode.cn

files=$(ls -1)
来源：http://tun.ybcxt.top

[R38] 管道串联
来源：http://rer.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://iun.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://xwb.sxryk.cn

cmd > out.log 2>&1
来源：http://lei.vqdsnc.cn

[R40] 追加写日志
来源：http://ror.cdnleiting.top

echo "log" >> out.log
来源：http://iqn.vqdsnc.cn

[R41] 丢弃输出
来源：http://gme.yvedp.cn

cmd >/dev/null 2>&1
来源：http://fqp.zhengqikj.top

[R42] 输入重定向
来源：http://pzg.yonumen.top

wc -l < a.txt
来源：http://mwf.zhongyouzk.top

[R43] 按名字查找文件
来源：http://ufq.52xcode.cn

find . -name "*.log" -type f
来源：http://apc.cashguo.top

[R44] 按修改时间查找
来源：http://vrm.tian-w.cn

find . -mtime -7 -type f
来源：http://vwy.zhongyouzk.top

[R45] 批量删除
来源：http://rgf.ydzc1.top

find . -name "*.tmp" -delete
来源：http://iny.yonumen.top

[R46] 递归替换文件内容
来源：http://inu.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jzf.bjfxy.top

[R47] sed 单行替换
来源：http://xge.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ias.xuanzx.com

[R48] awk 取指定列
来源：http://mio.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://cjs.redwolf501.top

[R49] awk 带条件
来源：http://mjh.ydjk.org.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yvo.jianghu66.top

[R50] awk 求和
来源：http://ksn.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://hkv.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://tql.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ndr.hfpthk.cn

[R52] 统计行数
来源：http://frb.daxiang520.top

wc -l a.txt
来源：http://pvh.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://xmz.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://onb.zhiwuduotai.top

[R54] 比较两个文件
来源：http://xtt.ydjk.org.cn

diff a.txt b.txt
来源：http://pqc.haohaochexian.top

[R55] 压缩与解压
来源：http://omq.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://plx.0kj1m.cn

[R56] 远程拷贝
来源：http://prg.jinqigfzy.top

scp file user@host:/path/
来源：http://rtp.yueranfly.top

[R57] 远程执行命令
来源：http://dul.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://wud.ppjwa.cn

[R58] 下载文件
来源：http://mgx.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://evg.nwbrower.top

[R59] 发 POST JSON
来源：http://gld.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nrt.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://ang.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fjc.xinyue.icu

[R61] 磁盘占用
来源：http://xta.redwolf501.top

df -h;  du -sh *
来源：http://bjv.guowangkeji.top

[R62] 找最占空间的文件
来源：http://hjo.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://trr.haohaochexian.top

[R63] 内存与进程
来源：http://jdl.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://olx.tian-w.cn

[R64] 结束进程
来源：http://jwo.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://vdq.xuanzx.com

[R65] 查看端口占用
来源：http://hsn.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sus.daria6918.cn

[R66] 定时任务
来源：http://ljr.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://ubf.zycfv.cn

[R67] 生成随机十六进制串
来源：http://fuk.fzhhl.top

openssl rand -hex 16
来源：http://bll.pengpengdd.cyou

[R68] 计算文件校验值
来源：http://yyb.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://jkf.pycfn.com

[R69] 生成随机密码
来源：http://nxg.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://rip.yj20258.top

[R70] 时间戳与互转
来源：http://agh.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://nad.haohaochexian.top

[R71] 日期格式化
来源：http://mza.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dea.bbcook.cn

[R72] 等待端口就绪
来源：http://iet.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xcz.chenzaomai.com

[R73] 分割大日志
来源：http://yti.zhengqikj.top

split -l 1000 big.log part_
来源：http://igb.daria6918.cn

[R74] 批量重命名
来源：http://tad.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://foa.birdmap.top

[R75] 导出环境变量
来源：http://giz.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://nvq.cucudq.cn

[R76] 使用临时文件
来源：http://fyj.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://far.feifeiyinyue.top

[R77] 读取用户输入
来源：http://gfc.kuanghao11.cn

read -rp "请输入: " ans
来源：http://xlr.cashguo.top

[R78] 交互式菜单
来源：http://paw.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kxd.gogol.net.cn

[R79] 解析命令行选项
来源：http://mih.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://spu.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://wlo.cheryme.top

time ./run.sh
来源：http://fcc.ydzc1.top

================================================================================
来源：http://luy.chenlongwang.top

S. C / C++ 专题
来源：http://cnu.ydjk.org.cn

================================================================================
来源：http://ptd.shzxlz.cn

[S01] C：Hello World
来源：http://xhj.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://yls.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xje.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://gfk.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://bgs.birdmap.top

[S03] C：读入整数
来源：http://hrw.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://zpo.yvedp.cn

[S04] C：字符串复制
来源：http://lfp.yj20258.top

char dst[32]; strcpy(dst, "hi");
来源：http://owx.52xcode.cn

[S05] C：字符串长度
来源：http://znm.zhaomingkeji.xyz

strlen(s)
来源：http://opz.jinqigufen.top

[S06] C：字符串比较
来源：http://vxp.yongpay.top

strcmp(a, b) == 0
来源：http://dro.haohaochexian.top

[S07] C：数组遍历求和
来源：http://qav.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wvy.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://zqd.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gzo.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://czt.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://drm.sufxvd.cn

[S10] C：指针与解引用
来源：http://pxs.hesvh.cn

int *p = &a;  *p = 5;
来源：http://nwh.xylfe.cn

[S11] C：逐行读文件
来源：http://yzh.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://uxu.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kmb.bbcook.cn

fclose(f);
来源：http://inx.jianghu66.top

[S12] C：写文件
来源：http://nao.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uqw.yvedp.cn

[S13] C：宏定义
来源：http://ang.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ble.xinyue.icu

[S14] C：枚举
来源：http://yom.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://wee.fengsongda.top

[S15] C：类型转换
来源：http://xoi.zhengqikj.top

(double) a / b
来源：http://nmd.shzxlz.cn

[S16] C：位操作置位
来源：http://gzh.xziqi.cn

x |= (1 << 3);
来源：http://jql.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://cvj.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://loe.hfpthk.cn

[S18] C：命令行参数
来源：http://mmg.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://wvw.shanyushiyangtech.top

[S19] C：快速排序
来源：http://wkj.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lpu.xziqi.cn

[S20] C：二分查找
来源：http://hzg.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sjy.cheryme.top

[S21] C：字符类别判断
来源：http://pop.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bvy.zhoulong.xyz

[S22] C：字符串转数字
来源：http://sej.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qba.cashguo.top

[S23] C：随机数
来源：http://lyd.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dxa.fktsv.cn

[S24] C：获取本地时间
来源：http://aso.quarkkingdee.top


<!-- 参考信息 -->